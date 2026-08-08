# GitHub share 仓库 · 通用上传指南（给任何环境下的 Kimi）

> 用途：把下面「提示词」部分整段复制，粘贴到任何一个新会话中——无论是本机的 Kimi Work、远端服务器上的 Kimi Claw，还是其他任何 AI 运行方式——对方都能按约定把文件上传到我的 GitHub share 仓库并生成公开访问链接。
> 整理日期：2026-08-08（v2：通用环境版）

---

## 提示词（从这里开始复制）

我（用户）有一个用于公开分享文件的 GitHub 仓库。当我说「**上传到我的 GitHub 上的 share 仓库**」时，请按以下约定执行。

### 基本信息

- 仓库：`https://github.com/butterfly0923/share`（**公开仓库**，GitHub Pages 已开启，分支 `main`）
- 文件 push 到 `main` 后，约 **1~2 分钟**部署生效，公开访问地址为：
  ```
  https://butterfly0923.github.io/share/<文件相对路径>
  ```
- URL 与仓库内文件路径一一对应、**大小写敏感**；`.html` 直接渲染成网页，二进制文件自动触发下载
- ⚠️ 这是公开仓库，**不要上传隐私数据、凭据或敏感文件**
- 完成后请把可访问的链接给我，方便我转发给朋友

### 第一步：判断你运行在哪种环境

**情况 A：你运行在用户自己的 PC 上（Kimi Work，Windows）**

本机已有克隆和缓存凭据，直接使用：
- 克隆目录：`C:\Users\Shawn Zhang\Documents\kimi\workspace\share`
- git 凭据已缓存在 Windows 凭据管理器，push 不需要任何授权
- 流程：把文件复制进克隆目录 → `git add` → `git commit` → push 被拒则先 `git pull origin main --rebase` → `git push origin main`

**情况 B：其他任何环境（Kimi Claw、远端服务器、Linux/macOS，或没有缓存凭据的机器）**

你**没有**现成的推送权限，需要先向我要一个 **GitHub Personal Access Token (PAT)**。请这样对我说：

> 「请你在 GitHub 上生成一个 fine-grained Personal Access Token（Settings → Developer settings → Personal access tokens → Fine-grained tokens），Repository access 只选 `butterfly0923/share` 这一个仓库，Permissions 里把 **Contents** 设为 **Read and write**，然后把 token 发给我。用完后你可以随时在同一个页面把它吊销（Revoke）。」

拿到 token 后，下面两种方式任选其一（**优先方式一**，不依赖 git）：

### 方式一：GitHub REST API 直传（推荐，任何有 curl 的环境都能用）

适合一次上传一两个文件，无需安装 git、无需克隆仓库。

```bash
TOKEN=<用户提供的PAT>

# 1. 把文件内容编码为 base64（单行）
#    Linux/macOS:   base64 -w0 文件名
#    Windows 可用:  py -c "import base64,sys;print(base64.b64encode(open(sys.argv[1],'rb').read()).decode())" 文件名

# 2. 上传（仓库内目标路径需要做 URL 编码，例如空格是 %20）
curl -X PUT \
  -H "Authorization: Bearer $TOKEN" \
  -H "Accept: application/vnd.github+json" \
  "https://api.github.com/repos/butterfly0923/share/contents/<URL编码后的目标路径>" \
  -d '{"message": "Add <文件名>", "content": "<base64内容>"}'
```

- 返回 JSON 中出现 `"content"` 和 `"commit"` 即成功
- **如果要覆盖同名旧文件**：先 `curl -H "Authorization: Bearer $TOKEN" https://api.github.com/repos/butterfly0923/share/contents/<路径>` 拿到该文件的 `"sha"`，然后在 PUT 的 JSON 里加 `"sha": "<拿到的sha>"`
- 注意保护 token：不要写进任何会上传的文件，不要回显到日志里；用完后提醒我吊销

### 方式二：git clone + token 推送（适合批量文件）

```bash
git clone "https://x-access-token:<PAT>@github.com/butterfly0923/share.git"
cd share
cp <要上传的文件> .
git add . && git commit -m "Add files"
git push origin main
```

push 被拒（远端有新提交）时先 `git pull origin main --rebase` 再 push。

### 第三步：验证

push/API 调用成功后等待 1~2 分钟，然后验证：

```bash
curl -s -o /dev/null -w "%{http_code}" "https://butterfly0923.github.io/share/<URL编码后的文件路径>"
```

返回 `200` 即部署完成，把这条链接交给我。

## 提示词（到这里结束）

---

## 附：这套机制的背景（2026-08-02 搭建）

1. GitHub 免费账号 `butterfly0923` 下的公开仓库 `share`；免费账号的公开仓库可正常开启 GitHub Pages（Settings → Pages → Source 选 `main` 分支根目录）
2. Pages 域名是 `github.io` 而非 `github.com`——这是 GitHub 的静态托管服务域名，仓库代码页 `github.com/.../blob/...` 链接不能直接预览，必须走 `github.io` 链接
3. 用户 PC（Kimi Work）上：仓库克隆在 workspace，凭据经 Git Credential Manager 缓存，可免密 push
4. 用户浏览器装有 Tampermonkey 脚本：在仓库 Code 页面的文件列表中自动给每行插入 "Deploy Link" 列，点击直达部署地址
5. 备选渠道曾评估：香港服务器（要密码，麻烦）、transfer.sh（被公司防火墙拦截）、Netlify Drop（可用，适合一次性拖拽）——最终采用 GitHub + Pages 方案：可版本管理、链接稳定、网页直开、二进制自动下载

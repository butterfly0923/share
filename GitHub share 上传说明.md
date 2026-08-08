# GitHub share 仓库 · 文件分享机制说明（提示词）

> 用途：把下面「提示词」部分整段复制，粘贴到任何一个新会话中（包括其他项目会话、网页版 Kimi、或其他 AI），对方就能按照约定帮你把文件上传到 GitHub share 仓库并生成公开访问链接。
> 整理日期：2026-08-08

---

## 提示词（从这里开始复制）

我（用户）有一个用于公开分享文件的 GitHub 仓库，当我说「**上传到我的 GitHub 上的 share 仓库**」时，请按以下约定执行：

### 基本信息

- 仓库地址：`https://github.com/butterfly0923/share`（**公开仓库**，GitHub Pages 已开启，分支为 `main`）
- 本机克隆位置：`C:\Users\Shawn Zhang\Documents\kimi\workspace\share`
- 本机 git 凭据已于 2026-08-02 授权并缓存（Windows 凭据管理器），`git push` 无需再向我索要账号密码或 token

### 标准操作流程

1. 把要分享的文件复制到本地克隆目录 `C:\Users\Shawn Zhang\Documents\kimi\workspace\share\` 中（保持我指定的文件名；可以放子目录，URL 路径与文件路径一致）
2. 在该目录执行：
   ```bash
   git add <文件名>
   git commit -m "Add <文件名>"
   git push origin main
   ```
3. 如果 push 被拒绝（远端有我通过网页上传的新提交），先执行 `git pull origin main --rebase`，再重新 push
4. push 成功后**等待约 1~2 分钟**（GitHub Pages 部署有延迟），文件即可通过以下地址公开访问：
   ```
   https://butterfly0923.github.io/share/<文件名>
   ```
5. 完成后把这条可访问的链接给我，方便我直接转发给朋友

### 访问行为说明

- `.html` 文件：浏览器中**直接渲染为网页**，适合分享报告、列表页
- 二进制文件（如 .dll、.zip）：访问链接时**自动触发下载**
- 文件名大小写敏感，URL 必须与文件名完全一致
- 仓库根目录放 `index.html` 可以让链接更短，但我一般保留原文件名，让这个仓库保持通用

### 注意事项

- 这是**公开仓库**，任何人都能访问——不要上传隐私数据、凭据或敏感文件
- 如果我要分享的文件在别的目录，先把文件复制到克隆目录再提交，不要移动原文件
- 我的浏览器装有配套 Tampermonkey 脚本，在仓库 Code 页面的文件列表里每行会显示 "Deploy Link"，点击直达部署后的地址——所以只需告诉我文件名即可，我可以自己核对链接

## 提示词（到这里结束）

---

## 附：这套机制是怎么搭起来的（背景记录，2026-08-02）

1. 在 GitHub 免费账号 `butterfly0923` 下新建公开仓库 `share`（免费账号的公开仓库可正常开启 GitHub Pages，无限制；Pages 域名是 `github.io` 而非 `github.com`，这是 GitHub 的静态托管服务域名）
2. 仓库 Settings → Pages → Source 选择 `main` 分支根目录，开启 GitHub Pages
3. 把仓库克隆到本机 workspace，第一次 `git push` 时通过 Git Credential Manager 完成授权并缓存凭据
4. 安装 Tampermonkey 脚本：精确匹配 `https://github.com/butterfly0923/share`，在文件列表表格中给每行插入 "Deploy Link" 列（链接拼接为 `https://butterfly0923.github.io/share/` + 文件名），同时在 thead 中补充对应表头，保持表头与表身列数一致

### 备选分享渠道对比

| 渠道 | 结果 |
|---|---|
| 香港服务器 | 默认需要密码，分享麻烦，弃用 |
| transfer.sh | 被公司防火墙拦截，不可用 |
| Netlify Drop | 可用，适合一次性拖拽分享 |
| **GitHub + Pages（本方案）** | ✅ 最终采用：可版本管理、链接稳定、网页直开、二进制自动下载 |

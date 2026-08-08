# 《无光之海》(Sunless Sea) 完全中文手册

> **版本**: 1.0  
> **整理日期**: 2026年8月  
> **资料来源**: Sunless Sea 官方 Wiki (sunlesssea.miraheze.org)、Failbetter Games 社区论坛、SteamAH 攻略站等  
> **说明**: 本手册基于英文社区资料翻译整理，游戏内专有名词均保留英文原名并附中文翻译。

---

## 目录

1. [游戏基本机制](#一游戏基本机制)
2. [任务指南](#二任务指南)
3. [物品列表](#三物品列表)
4. [地点与港口](#四地点与港口)
5. [船员与军官](#五船员与军官)
6. [附录](#六附录)

---

## 一、游戏基本机制

### 1.1 游戏概述

《无光之海》(Sunless Sea) 是由 Failbetter Games 开发的一款维多利亚哥特风格航海探险 RPG。游戏设定在《堕落伦敦》(Fallen London) 宇宙的地下海——**翁特之海 (Unterzee)**。玩家扮演一名船长，驾驶蒸汽船探索未知海域，面对疯狂、背叛、死亡与遗产继承。

### 1.2 核心属性

你的船长拥有五项核心属性：

| 英文 | 中文 | 作用 |
|------|------|------|
| **Iron** | 钢铁 | 增加武器伤害，战斗挑战 |
| **Veils** | 面纱 | 提高隐蔽性，避免被发现 |
| **Mirrors** | 镜子 | 扩大视野范围，发现隐藏事物 |
| **Hearts** | 心脏 | 对抗恐惧，船员管理挑战 |
| **Pages** | 书页 | 获取经验效率，知识挑战 |

**初始背景选择**（影响初始属性）：

| 背景 | 中文 | 属性加成 |
|------|------|----------|
| A street urchin | 街头顽童 | +Veils |
| A poet! | 诗人 | +Pages |
| A Veteran of the Campaign of '68 | '68战役老兵 | +Iron |
| An ordained priest | 受戒牧师 | +Hearts |
| A natural philosopher | 自然哲学家 | +Mirrors |
| A Past Wreathed In Shadows | 阴影缠绕的过去 | 无初始加成，可后续选择 |

### 1.3 船只系统

#### 1.3.1 船只属性

每艘船有以下属性：

- **Hull (船体)**: 船只的生命值。新手起始为 75。
- **Hold (货舱)**: 载货容量。新手船为 40。
- **Quarters (船员舱)**: 容纳船员数量。新手船为 10。
- **Ship Weight (船重)**: 影响移动速度，越重越慢。
- **Engine Power (引擎功率)**: 由引擎决定。

#### 1.3.2 装备槽位

每艘船有 4-6 个装备槽位：

| 槽位 | 说明 | 可用船只 |
|------|------|----------|
| **Deck** | 甲板武器 | 所有船只 |
| **Engine** | 引擎 | 所有船只 |
| **Bridge** | 舰桥设备 | 所有船只 |
| **Auxiliary** | 辅助设备 | 所有船只 |
| **Forward** | 船首武器 | 部分船只 |
| **Aft** | 船尾设备 | 部分船只 |

> **注意**: 装备只能在港口更换。出售价格通常为购入价的 50%。

#### 1.3.3 船只列表

| 英文名称 | 中文 | 船体 | 货舱 | 船员 | 槽位 | 价格 | 属性加成 |
|----------|------|------|------|------|------|------|----------|
| **Ligeia-class Steamer** | 利盖亚级蒸汽船 | 75 | 40 | 10 | 4 | 免费(初始) | 无 |
| **Phorcyd-class Corvette** | 福基德级护卫舰 | 200 | 40 | 15 | 5 | 4,000 E | 无 |
| **Maenad-class Frigate** | 梅纳德级驱逐舰 | 450 | 70 | 25 | 6 | 15,000 E | +5 Iron, +5 Mirrors |
| **Caligo-class Merchant Cruiser** | 卡利戈级商船 | 300 | 120 | 30 | 5 | 8,000 E | 无 |
| **Eschatologue-class Dreadnought** | 末日级无畏舰 | 600 | 100 | 40 | 6 | 30,000 E | +10 Iron, -10 Veils |
| **Lampad-class Cutter** | 兰帕德级快艇 | 50 | 20 | 5 | 4 | 500 E | +10 Veils |
| **Stymphalos-class Steam Launch** | 斯廷法利斯级蒸汽艇 | 1 | 10 | 5 | 4 | 特殊 | 无 |

> **新手推荐**: Maenad-class Frigate（全能型）或 Caligo-class Merchant Cruiser（贸易型）。

### 1.4 资源管理

#### 1.4.1 核心资源

| 资源 | 说明 | 获取方式 |
|------|------|----------|
| **Fuel (燃料)** | 驱动蒸汽船 | 伦敦购买(20E)、各港口商店、战利品 |
| **Supplies (补给)** | 船员食物 | 伦敦购买(10E)、各港口商店、狩猎 |
| **Echoes (回声币)** | 游戏货币 | 贸易、任务奖励、战利品 |

#### 1.4.2 恐惧机制 (Terror)

- 在黑暗中航行、遭遇恐怖事件会增加 **Terror (恐惧)**
- 高恐惧会导致船员发疯、死亡或叛变
- 降低方法：靠近海岸航行、保持灯光开启、访问港口休息、某些军官能力
- 当 Terror 达到 100 时，会发生严重后果

#### 1.4.3 船员消耗

- 船员数量低于 50% 时，船速降至 1 档
- 补给不足时，船员会饿死
- 某些事件会消耗或损失船员

### 1.5 战斗系统

#### 1.5.1 战斗基础

- **照明弹 (Flares)**: 暴露敌人位置，但降低隐蔽性
- **潜行攻击 (Sneak Attack)**: 在敌人未发现时发动，造成额外伤害
- **尾行战术**: 保持在敌人后方，使用甲板武器攻击（对大型船只效果降低）

#### 1.5.2 武器类型

| 类型 | 特点 | 适用场景 |
|------|------|----------|
| **Cannons (火炮)** | 标准武器，平衡型 | 通用 |
| **Torpedoes (鱼雷)** | 高伤害，射程短 | 尾行战术 |
| **Harpoons (鱼叉)** | 中等伤害，特殊效果 | 狩猎海兽 |
| **Deck Guns (甲板炮)** | 射程远，适合追击 | 船尾攻击 |

### 1.6 遗产继承系统

当你死亡或退休时，下一代船长可以继承：

- 部分属性（通过 Legacy 物品）
- 部分金钱
- 已探索的地图（海岸线）
- 某些特殊物品

---

## 二、任务指南

### 2.1 主线任务 (Ambitions)

游戏开始时可选 3 个初始 Ambition，游戏过程中可解锁 3 个隐藏 Ambition。

#### 2.1.1 Your Father's Bones（父亲的遗骨）

| 项目 | 内容 |
|------|------|
| **类型** | 初始 Ambition |
| **目标** | 找到你父亲的遗骨并带回伦敦 |
| **流程** | 1. 在伦敦开始调查<br>2. 前往 Grand Geode 获取线索<br>3. 在 Chapel of Lights 找到遗骨<br>4. 带回伦敦安葬 |
| **奖励** | 完成 Ambition，解锁特殊遗产 |

#### 2.1.2 Fulfillment / Wealth（财富）

| 项目 | 内容 |
|------|------|
| **类型** | 初始 Ambition |
| **目标** | 积累 10,000 Echoes 并退休 |
| **流程** | 通过贸易、任务、狩猎积累财富，在伦敦 lodgings 选择退休 |
| **奖励** | 退休结局，财富传承 |

#### 2.1.3 A Private Kingdom（私人王国）

| 项目 | 内容 |
|------|------|
| **类型** | 隐藏 Ambition |
| **目标** | 在 Aestival 岛建立殖民地并宣布独立 |
| **流程** | 1. 发现 Aestival 岛<br>2. 建立 Your Colony<br>3. 将人口增加到 77+<br>4. 任命一名军官为 Viceroy<br>5. 选择 "Declare yourself a nation" |
| **奖励** | 特殊胜利结局，可获得任何遗产物品 |

#### 2.1.4 The Uttermost East（极东之地）

| 项目 | 内容 |
|------|------|
| **类型** | 隐藏 Ambition |
| **目标** | 跟随 Carnelian Exile 前往极东 |
| **流程** | 1. 在 Frostfound 获取 Burning Name<br>2. 完成一系列艰难挑战<br>3. 前往 Irem<br>4. 最终牺牲大量属性和物品 |
| **奖励** | 特殊胜利结局，保留 Hearts 属性的一半传承 |

#### 2.1.5 Immortality（不朽）- Zubmariner DLC

| 项目 | 内容 |
|------|------|
| **类型** | Zubmariner DLC Ambition |
| **目标** | 追寻 Seven Against Nidah 获得不朽 |
| **流程** | 1. 找到 Seven 成员<br>2. 前往 Nidah（Presbyterate 中心）<br>3. 选择：与 Seven 一同进入、背叛他们、或站在 Presbyterate 一方 |
| **奖励** | 多种结局，不朽或王国 |

### 2.2 重要支线任务 (Storylets)

#### 2.2.1 The Trouble with Tomb-Colonists（坟民之旅）

| 项目 | 内容 |
|------|------|
| **起始** | 伦敦，接载一名 Tomb-Colonist |
| **目标** | 将 12 名 Tomb-Colonist 运送到各地，最终带回 Venderbight |
| **需要物品** | 12 x Supplies, 10 x Cask of Mushroom Wine（诗人背景） |
| **关键地点** | Shepherd's Wash, Gaider's Mourn, Khan's Glory, Polythreme, Irem, Chelonate |
| **奖励** | 12名全活：1 x Judgements' Egg + 1500 Echoes |

#### 2.2.2 The Vengeance of Jonah（约拿的复仇）

| 项目 | 内容 |
|------|------|
| **相关** | Bandaged Poissonnier 招募任务 |
| **地点** | Venderbight |
| **流程** | 完成一系列事件，最终花费 300 Echoes 招募 Bandaged Poissonnier |
| **奖励** | 招募厨师军官 |

#### 2.2.3 The Pulse of the Principles（珊瑚法则的脉动）

| 项目 | 内容 |
|------|------|
| **相关** | Nacreous Outcast 招募任务 |
| **流程** | 完成 Principles of Coral 相关事件链 |
| **关键** | 选择 "An Extra Move" 招募 Nacreous Outcast |
| **奖励** | 招募稀有军官 |

#### 2.2.4 The Merchant Venturer（商人的冒险）

| 项目 | 内容 |
|------|------|
| **目标** | 跟随商人前往 Avid Horizon |
| **结局** | 选择 "Pass beyond with him" 离开地球，进入 High Wilderness |
| **奖励** | 特殊结局 |

#### 2.2.5 The Soaring Glory（齐柏林飞艇）

| 项目 | 内容 |
|------|------|
| **地点** | Empire of Hands |
| **目标** | 建造中的齐柏林飞艇 |
| **结局** | 选择 "Steal the Zeppelin" 偷走飞艇向东飞行 |
| **奖励** | 特殊结局（与 The Uttermost East 不同） |

### 2.3 贸易路线

#### 2.3.1 新手贸易路线

| 路线 | 货物 | 利润 |
|------|------|------|
| 伦敦 → Venderbight | 坟民 | 基础收入 |
| Salt Lions → 伦敦 | Sphinxstone | 高额利润（需投资 200E） |
| 伦敦 → Port Carnelian | 蘑菇酒 | 中等利润 |
| Surface → 伦敦 | 阳光（Mirrorcatch Boxes）| 高风险高利润 |

#### 2.3.2 后期贸易路线

| 路线 | 货物 | 利润 |
|------|------|------|
| Port Carnelian → Chelonate | 蓝宝石 | 13E/单位 |
| Empire of Hands → Irem | 咖啡 → 帕拉波拉亚麻 | 39E/单位利润 |
| Mangrove College Wisp-Ways | 蜡烛 → 珍宝 | 高价值物品 |
| 地表（Surface） | Darkdrop Coffee | 极高利润 |

---

## 三、物品列表

### 3.1 装备 (Ship Equipment)

#### 3.1.1 武器 (Weapons) - 共 17 种

| 英文名称 | 中文翻译 | 槽位 | 属性/效果 | 获取方式 |
|----------|----------|------|-----------|----------|
| **Caminus Yards Helltrasher** | 卡米努斯船厂地狱撕裂者 | Deck | 高伤害 | 伦敦购买 |
| **Memento Mori** | 勿忘你终有一死 | Forward | 极高伤害，红色光束 | Irrepressible Cannoneer 任务 |
| **Icarus in Black** | 黑伊卡洛斯 | Forward | 末日伤害，发射猎人 | 特殊任务 |
| **Judgement Resonator** | 审判共振器 | Forward | 高伤害 | 伦敦购买 |
| **Reproach** | 谴责 | Deck | 新手武器 | 起始装备/购买 |
| **Harpoons** | 鱼叉 | Deck | 狩猎专用 | 各港口 |
| **Torpedoes** | 鱼雷 | Forward/Deck | 高伤害，短射程 | 各港口 |
| **Cannon** | 火炮 | Deck/Forward | 标准武器 | 各港口 |
| **Flare Gun** | 信号枪 | Auxiliary | 照明弹 | 起始装备 |

#### 3.1.2 引擎 (Engines) - 共 8 种

| 英文名称 | 中文翻译 | 功率 | 燃料效率 | 价格 | 备注 |
|----------|----------|------|----------|------|------|
| **Old Engine** | 老旧引擎 | 低 | 低 | 免费 | 起始装备 |
| **Caminus Yards 'Compulsion'** | 卡米努斯船厂'强迫' | 中 | 中 | ~1000E | 标准升级 |
| **Caminus Yards 'Durendal'** | 卡米努斯船厂'杜兰达尔' | 高 | 中 | ~3000E | 高速引擎 |
| **We Are Clay** | 我们是黏土 | 特殊 | 极高 | 任务获取 | 黏土人引擎，低维护 |
| **Maybe's Daughter** |  Maybe 之女 | 中 | 高 | 任务获取 | 平衡型 |
| **The Serpentine** | 蛇形 | 高 | 低 | ~5000E | 快速但耗油 |
| **The Elder** | 长者 | 极高 | 低 | ~8000E | 最高功率 |
| **Avid Suppressor** |  Avid 抑制器 | Aft | - | ~2000E | 实际为 Aft 设备，提供速度加成 |

#### 3.1.3 其他装备 (Miscellaneous) - 共 20 种

| 英文名称 | 中文翻译 | 槽位 | 属性加成 | 获取方式 |
|----------|----------|------|----------|----------|
| **The Zong of the Zee** | 海之宗 | Bridge | +10 全属性 | 任务制造（需 77 Zee-ztory） |
| **Dawn's Law** | 黎明法则 | Auxiliary | 抑制阳光伤害 | 特殊任务 |
| **Milebreaker** | 破里器 | Aft | +10% 燃料效率 | 伦敦购买 |
| **Suppressor** | 抑制器 | Aft | 减少引擎噪音 | 伦敦购买 |
| **Weeping Scar** | 哭泣伤疤 | Bridge | +Veils | 特殊事件 |
| **Boke of Sharps** | 锐器之书 | Bridge | +Iron | 特殊事件 |
| **The Cladery Heart** | 克拉德里之心 | Auxiliary | 治疗相关 | Cladery Heir 任务 |
| **Scrimshander Carving Knife** | 斯克里姆尚德雕刻刀 | - | 工具 | 特殊任务 |

### 3.2 货物 (Cargo / Trade Goods)

| 英文名称 | 中文翻译 | 基础价格 | 常见来源 | 常见销路 |
|----------|----------|----------|----------|----------|
| **Fuel** | 燃料 | 20E | 伦敦、各港口 | 通用 |
| **Supplies** | 补给 | 10E | 伦敦、各港口 | 通用 |
| **Sphinxstone** | 斯芬克斯石 | 高 | Salt Lions | 伦敦 |
| **Mushroom Wine** | 蘑菇酒 | 15E | 伦敦 | Port Carnelian |
| **Cask of Mushroom Wine** | 桶装蘑菇酒 | 150E | 伦敦 | 各港口 |
| **Coffee** | 咖啡 | 40E | Khan's Heart | Irem |
| **Darkdrop Coffee** | 黑滴咖啡 | 高 | Port Carnelian | Surface |
| **Sapphires** | 蓝宝石 | 高 | Port Carnelian | Chelonate |
| **Red Honey** | 红蜜 | 高 | Isle of Cats | 伦敦 |
| **Sunlight** | 阳光 | 极高 | Surface（Mirrorcatch Box）| 伦敦/Isle of Cats |
| **Parabola-Linen** | 帕拉波拉亚麻 | 高 | Irem | 各港口 |
| **Judgements' Egg** | 审判之蛋 | 极高 | 任务奖励 | 出售/收藏 |
| **Hunting Trophy** | 狩猎战利品 | 65E | 海兽 | Chelonate等 |
| **Outlandish Artefact** | 异域文物 | 100E | 探索 | 伦敦 |
| **Recent News** | 最新消息 | 10E | 伦敦 | 各港口 |
| **Strange Catch** | 奇异捕获 | 变 | 钓鱼 | 各港口 |
| **Amber** | 琥珀 | 变 | 探索 | 各港口 |
| **Doomed Monster-Hunter** | 注定的怪物猎人 | 特殊 | 特殊 | Icarus in Black 弹药 |

### 3.3 奇珍 (Curiosities)

| 英文名称 | 中文翻译 | 用途 | 获取方式 |
|----------|----------|------|----------|
| **Secret** | 秘密 | 提升属性、任务需要 | 探索、任务、击杀 |
| **Fragment** | 碎片 | 合成 Secret | 各种活动 |
| **Memory of Distant Shores** | 遥远海岸的记忆 | 任务、交易 | 探索 |
| **Tale of Terror!!** | 恐怖故事!! | 任务、交易 | 事件 |
| **Zee-ztory** | 海之故事 | 任务、写 Zong of the Zee | 探索、击杀 |
| **Lamentable Relic** | 可悲的遗物 | 出售 | 击杀 |
| **A Port Report** | 港口报告 | 交给 Admiralty | 访问港口 |
| **Admiralty Favour** | 海军部 favor | 修船折扣 | 提交港口报告 |
| **Terror** | 恐惧 | 负面状态 | 黑暗、恐怖事件 |
| **Hunger** | 饥饿 | 负面状态 | 缺补给 |
| **Wounds** | 伤害 | 负面状态 | 战斗、事件 |
| **Yearning, Burning** | 渴望，燃烧 | 危险状态（阳光相关）| 填充 Mirrorcatch Box |
| **Something Awaits You** | 某事待你 | 触发港口特殊事件 | 海上航行时间 |
| **Another Day: A New Recruit?** | 又一天：新招募？ | 招募军官 | 伦敦抵达时拥有 Something Awaits You |

### 3.4 任务物品 (Quest Items)

| 英文名称 | 中文翻译 | 相关任务 |
|----------|----------|----------|
| **The Vengeance of Jonah** | 约拿的复仇 | Bandaged Poissonnier 招募 |
| **The Pulse of the Principles** | 珊瑚法则的脉动 | Nacreous Outcast 招募 |
| **An Extra Move** | 额外一步 | Nacreous Outcast 招募 |
| **Burning Name** | 燃烧之名 | The Uttermost East |
| **Objective: Tomb-Colonists** | 目标：坟民 | The Trouble with Tomb-Colonists |
| **Objective: Ambition** | 目标：Ambition | 主线追踪 |

---

## 四、地点与港口

### 4.1 核心区域

#### 4.1.1 Fallen London（堕落伦敦）

| 项目 | 内容 |
|------|------|
| **位置** | 地图中央，你的起始港口 |
| **设施** | Wolfstack Docks（码头）、Your Lodgings（住所）、The University（大学）、Admiralty（海军部）、Caminus Yards（造船厂） |
| **商店** | Mrs Plenty's Shipside Provisioners（补给）、Wolfstack Exchange（交易所）、Carrow's Naval Surplus（海军剩余物资）、Caminus Yards（武器装备）、The Iron & Misery Company（铁与苦难公司）、Bultitude's House of Vision（视觉之家） |
| **特色** | 游戏中心枢纽，可修船、招募军官、购买装备、提交港口报告 |

#### 4.1.2 Venderbight（文德拜特）

| 项目 | 内容 |
|------|------|
| **位置** | 伦敦北方 |
| **特色** | Tomb-Colonies（坟民殖民地），可交付坟民 |
| **招募** | Bandaged Poissonnier（通过 The Vengeance of Jonah） |

### 4.2 Unterzee 港口列表

#### 北方 (The North)

| 英文 | 中文 | 特色 |
|------|------|------|
| **Whither** | 凋零之地 | 知识港口，可获得 Zee-ztory |
| **Codex** | 法典 | 沉没的城市 |
| **The Avid Horizon** | 热切的 Horizon | 世界边缘 |

#### 东北方 (The Northeast)

| 英文 | 中文 | 特色 |
|------|------|------|
| **The Salt Lions** | 盐之狮 | 两个巨大的斯芬克斯，Sphinxstone 来源 |
| **The Grand Geode** | 大晶洞 | 与 A Private Kingdom Ambition 相关 |

#### 东方 (The East)

| 英文 | 中文 | 特色 |
|------|------|------|
| **Irem** | 伊瑞姆 | 梦境港口，可用 Coffee 换 Parabola-Linen |
| **The Chelonate** | 海龟之国 | 巨大的海龟背上的国家，可交易 Hunting Trophy |
| **The Principles of Coral** | 珊瑚法则 | 水下城市（Zubmariner） |

#### 东南方 (The Southeast)

| 英文 | 中文 | 特色 |
|------|------|------|
| **Port Carnelian** | 红玉髓港 | 蓝宝石产地，咖啡贸易 |
| **Khan's Heart** | 可汗之心 | Khanate 首都，重要贸易中心 |
| **Khan's Shadow** | 可汗之影 | 黑市，可出售各种物品 |
| **Khan's Glory** | 可汗之荣耀 | 军事港口 |
| **Gaider's Mourn** | 盖德之哀 | 海盗港 |
| **The Isle of Cats** | 猫岛 | 红蜜产地 |

#### 南方 (The South)

| 英文 | 中文 | 特色 |
|------|------|------|
| **The Iron Republic** | 铁之共和国 | 混乱之城，法律由市民投票决定 |
| **Mt. Palmerston** | 帕尔默斯顿山 | 火山 |
| **Adam's Way** | 亚当之路 | 通往 Elder Continent 的入口 |
| **Aestival** | 夏至岛 | 可建立殖民地（A Private Kingdom） |
| **The Uttershroom** |  uttershroom | 巨大蘑菇 |

#### 西南方 (The Southwest)

| 英文 | 中文 | 特色 |
|------|------|------|
| **The Dawn Machine** | 黎明机器 | 人造太阳，危险区域 |
| **The Grand Geode** | 大晶洞 | （重复？需确认） |
| **Frostfound** | 霜之 found | 冰冻废墟，获取 Burning Name |

#### 西方 (The West)

| 英文 | 中文 | 特色 |
|------|------|------|
| **Hunter's Keep** | 猎人小屋 | 提供庇护 |
| **Mutton Island** | 羊肉岛 | 靠近伦敦，蘑菇酒产地 |
| **The Shepherd Isles** | 牧羊人群岛 | 可交易 Zee-ztory |

#### 西北方 (The Northwest)

| 英文 | 中文 | 特色 |
|------|------|------|
| **The Tomb-Colonies** | 坟民殖民地 | 古老文明遗迹 |
| **The Unterzee** | 翁特之海深处 | 各种随机遭遇 |

### 4.3 Zubmariner DLC 新增地点

| 英文 | 中文 | 特色 |
|------|------|------|
| **Dahut** | 达胡特 | 溺亡者之城 |
| **Wrack** | 残骸 | 沉船之城 |
| **Anthe** | 安特 | 开花水晶之城 |
| **Scrimshander** | 斯克里姆尚德 | 象牙与历史之城 |
| **Nook** |  nook | 牙齿 |
| **Aigul** | 艾古尔 | 尖刺要塞 |
| **Hideaway** | 藏身处 | 巨龟背上的机械城 |
| **Low Barnet** | 低巴尼特 | 沉没郊区，Drownie 聚集地 |
| **The Gant Pole** | 甘特极 | 口袋表死去的地方 |
| **The Fathomking's Hold** | 深渊之王领地 | 水下王国 |
| **Nidah** | 尼达 | 不朽之城（Presbyterate 中心） |

### 4.4 特殊地点

| 英文 | 中文 | 说明 |
|------|------|------|
| **The Surface** | 地表 | 可通过 Cumaean Canal 到达 |
| **Vienna** | 维也纳 | 可通过 Avernus 到达 |
| **Naples** | 那不勒斯 | 地表城市 |
| **Avernus** | 阿维努斯 | 通往地表的入口 |
| **The Cumaean Canal** | 库迈运河 | 连接 Neath 与地表 |

---

## 五、船员与军官

### 5.1 军官系统概述

- **军官 (Officers)** 不占用船员名额
- 每位军官占据一个职位，提供属性加成
- 更换军官会 +1 Terror
- 在伦敦可通过 "A new recruit!" 招募（需要 Something Awaits You）
- 部分军官可通过任务招募

### 5.2 可招募军官列表

#### 厨师 (Cook)

| 英文名称 | 中文 | 属性加成 | 训练上限 | 招募地点 | 招募条件 |
|----------|------|----------|----------|----------|----------|
| **Bandaged Poissonnier** | 绷带鱼贩 | +6 Hearts, +3 Pages | Hearts 100 | Venderbight | 完成 The Vengeance of Jonah，花费 300E |
| **Bandaged Chef-Paramount** | 绷带主厨 | +9 Hearts, +5 Pages | Hearts 150 | 晋升 | Bandaged Poissonnier 晋升 |

#### 工程师 (Engineer)

| 英文名称 | 中文 | 属性加成 | 训练上限 | 招募地点 | 招募条件 |
|----------|------|----------|----------|----------|----------|
| **Tireless Mechanic** | 不知疲倦的机械师 | +6 Mirrors, +3 Iron | Mirrors 100 | 伦敦随机招募 | 通过 "A new recruit!" |

#### 大副 (First Officer)

| 英文名称 | 中文 | 属性加成 | 训练上限 | 招募地点 | 招募条件 |
|----------|------|----------|----------|----------|----------|
| **Carnelian Exile** | 红玉髓流放者 | 特殊 | - | 特殊 | The Uttermost East 相关 |
| **Sigil-Ridden Navigator** | 印记导航员 | +6 Veils, +3 Mirrors | Veils 100 | 特殊 | 完成特定故事线 |

#### 炮手 (Gunner)

| 英文名称 | 中文 | 属性加成 | 训练上限 | 招募地点 | 招募条件 |
|----------|------|----------|----------|----------|----------|
| **Irrepressible Cannoneer** | 不可抑制的炮手 | +6 Iron, +3 Hearts | Iron 100 | 特殊 | 完成任务 |

#### 医生 (Surgeon)

| 英文名称 | 中文 | 属性加成 | 训练上限 | 招募地点 | 招募条件 |
|----------|------|----------|----------|----------|----------|
| **Nacreous Outcast** | 珠母流放者 | +4 Hearts, +2 Pages, +2 Mirrors | Hearts 150 | Principles of Coral | 完成 The Pulse of the Principles，选择 An Extra Move |
| **Nacreous Survivor** | 珠母幸存者 | +8 Hearts, +4 Pages, +4 Mirrors | - | 晋升 | Nacreous Outcast 晋升 |

#### 其他军官

| 英文名称 | 中文 | 属性加成 | 训练上限 | 招募地点 | 招募条件 |
|----------|------|----------|----------|----------|----------|
| **Cladery Heir** | 克拉德里继承人 | 特殊 | - | 特殊 | 相关任务 |
| **Maybe's Daughter** | Maybe 之女 | 特殊 | - | 特殊 | 任务获取 |
| **The Campaigner** | 竞选者 | +Hearts | - | 伦敦 | 随机招募 |
| **The Presbyterate Adventuress** | 长老会女冒险家 | +Iron | - | 特殊 | 任务 |

### 5.3 吉祥物 (Mascots)

| 英文名称 | 中文 | 效果 | 招募地点 |
|----------|------|------|----------|
| **The Elegiac Cockatoo** | 挽歌鹦鹉 | +Hearts | 特殊事件 |
| **The Wretched Mog** | 可怜猫 | 特殊 | 特殊事件 |
| **The Satisfied Magician's Rabbit** | 满足魔术师的兔子 | 特殊 | 特殊事件 |

### 5.4 招募技巧

1. **伦敦招募**: 返回伦敦时如果拥有 Something Awaits You，可能出现 "A new recruit!" 选项
2. **任务招募**: 部分军官需要完成特定任务链才能招募
3. **晋升**: 部分军官可以通过训练晋升到更强版本
4. **避免重复**: 早期不要招募相同职位的军官（如两个厨师），因为只能使用一个

---

## 六、附录

### 6.1 敌人与危险

#### 6.1.1 初级敌人

| 英文 | 中文 | 生命值 | 特点 |
|------|------|--------|------|
| **Pirate Steam-Pinnacle** | 海盗蒸汽尖塔 | 30 HP | 容易潜行攻击，有宝箱 |
| **Crack Pirate Steam-Pinnacle** | 精英海盗蒸汽尖塔 | 80 HP | 更强版本 |
| **Bat Swarm** | 蝙蝠群 | 20 HP | 成群出现 |
| **Crab** | 螃蟹 | 20 HP | 新手猎物 |
| **Alcaeus-Class Corvette** | 阿尔凯乌斯级护卫舰 | 180 HP | Pirate-Poet 的船 |

#### 6.1.2 中级敌人

| 英文 | 中文 | 生命值 | 特点 |
|------|------|--------|------|
| **Pirate Frigate** | 海盗驱逐舰 | 90 HP | 标准海盗船 |
| **Unfinished Pirates** | 未完成海盗 | 75 HP | 出现在 Polythreme 附近 |
| **Faustic Corsair** | 浮士德海盗 | 300 HP | 出现在 Mt. Palmerston 附近 |
| **Western Antler-Crab** | 西方鹿角蟹 | 300 HP | 出现在 Uttershroom 附近 |
| **Lifeberg** | 生命冰山 | 高 HP | 撞击攻击 |

#### 6.1.3 高级敌人

| 英文 | 中文 | 生命值 | 特点 |
|------|------|--------|------|
| **Elder Crab** | 远古蟹 | 600 HP | 出现在 Aestival 附近 |
| **Mount Nomad** | 游牧山 | 极高 | Boss 级 |
| **Tree of Ages** | 时代之树 | 极高 | Boss 级 |
| **Unfinished Revolutionaries** | 未完成革命者 | 210 HP | 出现在 Iron Republic 附近 |

#### 6.1.4 Zubmariner 新增水下敌人

| 英文 | 中文 | 生命值 | 特点 |
|------|------|--------|------|
| **Corsair Undergalley** | 海盗水下划艇 | 30 HP | 易猎物 |
| **Putterpony** | 嗅探艇 | 120 HP | Khanate 船只，非敌对 |
| **Boundling** | 束缚者 | 220 HP | 水下束缚鲨 |
| **Beloved** | 被爱者 | 180 HP | 出现在 Wrack 附近 |
| **Constant Companion** | 永恒伴侣 | 高 | Zubmariner Boss |

### 6.2 实用技巧

#### 6.2.1 新手建议

1. **早期赚钱**: 接坟民去 Venderbight，探索新港口获取港口报告
2. **属性提升**: 优先提升 Iron（战斗）和 Veils（隐蔽）
3. **保存游戏**: 在进行危险任务前保存
4. **灯光管理**: 平衡灯光（降低 Terror）和隐蔽性（避免战斗）
5. **修船时机**: 船体降至 50-60% 时修理

#### 6.2.2 进阶技巧

1. **尾行战术**: 保持在敌船后方，使用 Deck 武器攻击
2. **阳光走私**: 使用 Mirrorcatch Box 在地表收集阳光出售（注意 Yearning, Burning）
3. **Wisp-Ways**: 在 Mangrove College 使用蜡烛换取高价值物品
4. **狩猎**: 击杀 Zee-beasts 获取 Hunting Trophy，在 Chelonate 换取高价物品
5. **军官搭配**: 为每个职位配备一名军官，最大化属性加成

#### 6.2.3 属性提升方法

| 属性 | 提升方法 |
|------|----------|
| Iron | 使用武器、完成战斗挑战、Boke of Sharps |
| Veils | 隐蔽行动、Weeping Scar、某些船只 |
| Mirrors | 观察、Tireless Mechanic、Mirrors 装备 |
| Hearts | 照顾船员、Bandaged Poissonnier、Hearts 装备 |
| Pages | 阅读、完成任务、Bandaged Poissonnier、Pages 装备 |

### 6.3 重要游戏机制

#### 6.3.1 Something Awaits You

- 在海上航行一段时间后会获得此状态
- 用于触发港口的特殊事件
- 是招募军官的必要条件

#### 6.3.2 Port Reports（港口报告）

- 访问新港口时自动获得
- 提交给伦敦 Admiralty 获得 Echoes 和 Favour
- 是早期重要收入来源

#### 6.3.3 Map 机制

- 每次新游戏，海岸线位置固定，但内陆地点随机
- 死亡后，下一代船长继承海岸线地图
- 使用 Zee-bat 或观察发现新地点

#### 6.3.4 Menaces（威胁）

| 威胁 | 效果 | 降低方法 |
|------|------|----------|
| **Terror** | 恐惧过高导致疯狂 | 灯光、靠近海岸、港口休息 |
| **Hunger** | 饥饿消耗船员 | 补充 Supplies |
| **Wounds** | 伤害导致死亡 | 休息、治疗 |
| **Suspicion** | 怀疑导致麻烦 | 避免非法活动 |
| **Yearning, Burning** | 阳光渴望 | 避免阳光、休息 |

### 6.4 推荐装备搭配

#### 6.4.1 新手搭配（Ligeia-class）

| 槽位 | 装备 | 说明 |
|------|------|------|
| Deck | Reproach（谴责） | 200E 购买的基础火炮 |
| Engine | 升级引擎 | Caminus Yards 'Compulsion' |
| Bridge | 属性装备 | 根据需求选择 |
| Auxiliary | Flare Gun | 起始装备 |

#### 6.4.2 战斗型搭配（Frigate）

| 槽位 | 装备 | 说明 |
|------|------|------|
| Forward | Memento Mori / Torpedoes | 高伤害 |
| Deck | Caminus Yards Helltrasher | 主力武器 |
| Aft | Avid Suppressor / Milebreaker | 速度/效率 |
| Engine | The Serpentine / The Elder | 高速 |
| Bridge | The Zong of the Zee | 全属性+10 |
| Auxiliary | Dawn's Law | 防护 |

#### 6.4.3 贸易型搭配（Merchant Cruiser）

| 槽位 | 装备 | 说明 |
|------|------|------|
| Deck | 标准火炮 | 自卫 |
| Aft | Milebreaker | 燃料效率+10% |
| Engine | We Are Clay / Maybe's Daughter | 高效率 |
| Bridge | 属性装备 | +Pages 用于探索 |
| Auxiliary | 辅助设备 | 根据需要 |

### 6.5 资源参考表

#### 6.5.1 常见物品价格

| 物品 | 购买价 | 出售价 | 备注 |
|------|--------|--------|------|
| Fuel | 20E | 10E | 基础资源 |
| Supplies | 10E | 5E | 基础资源 |
| Reproach | 200E | 100E | 新手武器 |
| Caminus Yards Helltrasher | ~1000E | ~500E | 标准武器 |
| Memento Mori | 任务 | - | 最强武器之一 |
| Milebreaker | ~2000E | ~1000E | Aft 设备 |
| Judgements' Egg | - | ~2500E | 高价值物品 |

#### 6.5.2 修船费用

| 船只 | 标准修船 | Admiralty Favour 修船 |
|------|----------|----------------------|
| Ligeia-class | ~100E | ~50E |
| Phorcyd-class | ~300E | ~150E |
| Maenad-class | ~700E | ~350E |
| Eschatologue-class | ~1000E | ~500E |

---

> **本手册完结**
> 
> 如有错误或遗漏，欢迎参考官方 Wiki: https://sunlesssea.miraheze.org/wiki/Main_Page
> 
> 祝各位船长在 Unterzee 的航行顺利——愿盐神保佑你们。🌊

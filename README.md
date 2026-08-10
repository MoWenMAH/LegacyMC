Status: Frozen until Jun 2027
(The server will remain up and running during this period)
这个服务器仍然运行，你可以随时进来

[English](#english) | [中文](#chinese)

---

<a name="english"></a>
## English

### I. Nonsense
By the time you see this project, I will have already uninstalled QQ and Discord, transferred all non-study-related files on my computer to an external hard drive, and handed it over to my dad for safekeeping. Today is August 9, 2026, with less than 10 months to go before the Gaokao (June 5, 2027). Time is flying by so fast. My high school days are coming to an end soon—it makes me so sad QwQ.

(For those unfamiliar with the Gaokao, you can think of it as an SAT taken by over 600,000 students, the New York Times wasn't exaggerating when it described it as 'thousands of troops crossing a single-log bridge. XD The Gaokao is immensely important to me—it not only determines whether I can get into a top-tier university, but also defines the future of both myself and my family. Plus, for me, I only get one shot at this.)

There's no need to elaborate on how critical and important it is, which is why I must put everything else on hold for the next 10 months to focus entirely on prep.
I've temporarily pushed all my projects to GitHub (including this one) so I can pick them back up after the Gaokao is over, starting after June 10, 2027.

### II. Introduction
This is a Minecraft Beta 1.7.3 modded server with custom plugins.

### III. Development Timeline
*(I will edit these experiences into a video and post it to YouTube after the Gaokao)*

- **(1) 2022**: Created custom modpacks for Beta 1.7.3 (see Fig. 1) and gathered resources, network and experience. This later evolved into the client for this project.
- **(2) July to August 2024**: Focused on server-side development. Got bukkit1060 core from GitHub, downloaded IC2 and BC backport for bukkit along with their prerequisites (ModloaderMP, Forge for bukkit) from mcarchive.org. Installed mods to the core and successfully launched it. (However, the server core wouldn't accept any config file tweaks. Deleting META-INF caused errors, and putting mods' .zip files into the mods folder also threw errors—the core was virtually impenetrable, acting like a completely locked-down jar.)
- **(3) 2025**:
  - **1. July**:
    - ① Analyzed the plugins needed for the server (Fig. 2) and got them from bukkit.org. Studied the guides left by each authors and debugged the individual plugins.
    - ② Installed several backported add-ons for IC2. (Ver 1.0.0)
  - **2. August 2**: Launched open beta.
- **(4) 2026**: *(Subsequent updates mostly focused on feature additions and bug fixes. For detailed changes, please refer to #dev-log)*
  - **1. February**:
    - ① Ver 1.1.0 (Since I couldn't find the Randman plugin (which relies on WorldBorder) back in July 2025, I had to generate random coordinates in 'the World' and use the Multiverse-Portals plugin to link 'the Lobby' to those coordinates to simulate random teleportation.)
    - ② Ver 1.1.1
  - **2. March**: Ver 1.2.0
  - **3. April**: Ver 1.2.1
  - **4. Jun 27**: Ver 1.2.2

### IV. Dev-log
- **Ver 0.0.0 | Jul - Aug 2024**
  - Set up CraftBukkit #1060 core (GitHub) and IC2, BC Bukkit backport (MCArchive.com).
- **Ver 1.0.0 | Aug 2, 2025**
  - 1. Started open beta
- **Ver 1.1.0 | February, 2026**
  - 1. Changed the Lobby. (Link: https://www.planetminecraft.com/project/castle-38/)
  - 2. Combined the Lobby with the World.
  - 3. Created a new world named "Skyland".
  - 4. Added Randman (Based on Worldborder) plugin for random world teleportation.
- **Ver 1.1.1 | February, 2026**
  - 1. Fixed a NoSuchMethodError triggered by snow melting
  - 2. Fixed an issue preventing OP from entering the Nether.
- **Ver 1.2.0 | March 2026**
  - 1. Removed 'the Skyland'.
  - 2. Added the iConomy plugin and built a shop.
  - 3. Creating a Residence plot now costs money.
- **Ver 1.2.1 | April 2026**
  - 1. Adjusted a WorldBorder configuration setting (timer-delay-ticks:) to achieve true random teleportation.
  - 2. Updated shop inventory.
- **Ver 1.2.2 | June 27, 2026**
  - 1. Installed two mods: IC2 Thermometer Port & Iron Chests Port.
- **Ver 1.2.3**
  - 1. Removed Multiverse and fixed the Nether access issues.

### V. Community
All modified plugin configurations and Ubuntu commands are available in the #opensource channel on our Discord server.

If you encounter any bugs or have feedback while playing, please open an issue in this repository.

Thank YOOOOU!!

---

<a name="chinese"></a>
## 中文

### 一、废话
当你看到这个项目时，我已经卸载了QQ和Discord，将计算机上所有与学习无关的文件传输到外部硬盘，并将其交给父母妥善保管。今天是2026年8月9日，离高考还有不到10个月的时间（2027年6月5日）。时间过得真快。我的高中生活很快就要结束了，这让我很伤心 QwQ。

（For those unfamiliar with the Gaokao, you can think of it as an SAT taken by over 600,000 students, the New York Times wasn't exaggerating when it described it as 'thousands of troops crossing a single-log bridge. XD The Gaokao is immensely important to me—it not only determines whether I can get into a top-tier university, but also defines the future of both myself and my family. Plus, for me, I only get one shot at this.)

没有必要详细说明它是多么的关键和重要，这就是为什么我必须在接下来的10个月里暂停所有其他事情，以完全专注于备考。
我已经暂时将我的所有项目推送到GitHub（包括这一个），以便在高考结束后（2027年6月10日之后）重新开始。

### 二、简介
这是一个带有自定义插件的 Minecraft Beta 1.7.3 Mod服务器。

### 三、发展时间表
*(我将把这些经历编辑成视频，并在高考结束后发布到YouTube)*

- **（1）2022年**：为 Beta 1.7.3 创建自定义 Mod包（见图1），并收集资源、网络和经验。这后来演变为该项目的客户端。
- **（2）2024年7月至8月**：专注于服务器端开发。从GitHub获得 bukkit1060 内核，从 mcarchive.org 下载了 bukkit 的 IC2 和 BC backport 及其先决条件（ModLoaderMP，Forge for bukkit）。将 Mod 安装到核心并成功启动。（然而，服务器核心不会接受任何配置文件调整。删除 META-INF 会导致错误，将 Mod 的 .zip 文件放入 mods 文件夹也会引发错误——核心几乎无法穿透，就像一个完全锁定的 jar。）
- **（3）2025年**：
  - **1. 7月**：
    - ① 分析服务器所需的插件（图2），并从 bukkit.org 获得它们。研究每个作者留下的指南，并调试各个插件。
    - ② 为 IC2 安装了几个移植版附加模组。（版本1.0.0）
  - **2. 8月2日**：发布开放测试版。
- **（4）2026年**：*(后续更新主要关注功能添加和错误修复。有关详细更改，请参阅#开发日志)*
  - **1. 2月**：
    - ① 1.1.0版（因为我在2025年7月找不到 Randman 插件（它依赖于 WorldBorder），所以我不得不在“世界”中生成随机坐标，并使用 Multiverse-Portals 插件将“大厅”链接到这些坐标，以模拟随机传送。）
    - ② 版本1.1.1
  - **2. 3月**：1.2.0版
  - **3. 4月**：1.2.1版
  - **4. 6月27日**：1.2.2版

### 四、开发日志
- **Ver 0.0.0 | 2024年7月-8月**
  - 设置 CraftBukkit #1060 核心（GitHub）和 IC2、BC Bukkit 移植版（MCArchive.com）。
- **1.0.0版 | 2025年8月2日**
  - 1. 开始开放测试版
- **Ver 1.1.0 | 2026年2月**
  - 1. 更改大厅。（链接：https://www.planetminecraft.com/project/castle-38/）
  - 2. 大厅与世界相结合。
  - 3. 创造了一个名为“Skyland”的新世界。
  - 4. 增加了 Randman（基于 WorldBorder）插件，用于随机世界传送。
- **Ver 1.1.1 | 2026年2月**
  - 1. 修复了融雪触发的 NoSuchMethodError
  - 2. 修复了一个阻止 OP 进入下界（Nether）的问题。
- **1.2.0版 | 2026年3月**
  - 1. 删除“Skyland”。
  - 2. 添加了 iConomy 插件，并建立了一个商店。
  - 3. 创建 Residence 领地地块现在需要花钱。
- **1.2.1版 | 2026年4月**
  - 1. 调整了 WorldBorder 配置设置（timer-delay-ticks:），以实现真正的随机传送。
  - 2. 更新商店库存。
- **1.2.2版 | 2026年6月27日**
  - 1. 安装了两个 Mod：IC2 Thermometer Port 和 Iron Chests Port。
- **Ver 1.2.3**
  - 1. 删除了 Multiverse 并修复了下界（Nether）访问问题。

### 五、社区
所有修改后的插件配置和 Ubuntu 命令都可以在 Discord 服务器上的 #opensource 频道中获得。

如果您在玩游戏时遇到任何 Bug 或有反馈，请在此存储库中打开 Issue。

谢谢你！！

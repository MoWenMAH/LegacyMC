Status: Frozen until Jun 2027
(The server will remain up and running during this period)
这个服务器仍然运行，你可以随时进来

[English](#english) | [中文](#chinese)

---

<a name="english"></a>
## English

### I. Nonsense
By the time you see this project, I will have already uninstalled QQ and Discord, transferred all non-study-related files on my computer to an external hard drive, and handed it over to my parents for safekeeping. Today is August 9, 2026, with less than 10 months to go before the Gaokao (June 5, 2027). Time is flying by so fast. My high school days are coming to an end soon—it makes me so sad QwQ.

(For those unfamiliar with the Gaokao, you can think of it as an SAT taken by over 600,000 students, the New York Times wasn't exaggerating when it described it as 'thousands of troops crossing a single-log bridge. XD The Gaokao is immensely important to me—it not only determines whether I can get into my favotite university, but also defines the future of both myself and my family. Plus, for me, I only get one shot at this.)

So I must put everything else on hold for the next 10 months to focus entirely on prep.
I've temporarily pushed all my projects to GitHub (this is one of them)so that I can pick them back up after the Gaokao is over, starting after June 10, 2027.

### II. Introduction
This is a Minecraft Beta 1.7.3 modded server with custom plugins,representing four years of total development and operation, plus one year in public beta.

### III. Development Timeline
*(I will edit these experiences into a video and post it to YouTube after the Gaokao)*

- **(1) 2022**: Created custom modpacks for Beta 1.7.3 (see Fig. 1) and gathered resources, network and experience. This later evolved into the client for this project.
- **(2) July to August 2024**: Focused on server-side development. Downloaded bukkit1060 core from GitHub, downloaded IC2 and BC backport for bukkit and their prerequisites (ModloaderMP, Forge for bukkit) from https://www.mcarchive.org. Installed mods to the core and successfully launched it. (However, the server core wouldn't accept any config file tweaks. Deleting META-INF caused errors, and putting mods' .zip files into the mods folder also threw errors—the core was virtually impenetrable, acting like a completely locked-down jar.)
- **(3) 2025**:
  - **1. July**:
    - ① Analyzed the plugins needed for the server (Fig. 2) and downloaded them from https://www.bukkit.org. Studied the guides left by each authors and debugged the individual plugins.
    - ② Installed several backported add-ons for IC2. (Ver 1.0.0)
    - (Since WorldGuard for Bukkit #1060 wasn't available at the time, and the Permissions plugin could only prevent block destruction globally by revoking the build permission for an entire group, I had to separate 'the World' and 'the Lobby' into two different worlds to protect the lobby).
  - **2. August 2**: Launched open beta.
  - (I rented a cloud server running Ubuntu and connected to it via Xshell."Back then, I thought SSH was strictly for remote access, just like Windows Remote Desktop. But later, while working with a dictionary pen (YDP031, running Android) (Figure 3), I realized SSH could also connect to a local OS. That's when it clicked for me: SSH is actually a tool for controlling an OS, and can be accessed by any OS. Describing it as a 'shell' is so spot on! XD.This later proved helpful when I was researching iOS downgrades)
  - Ubuntu commands:
  - sudo apt update
  - sudo apt install openjdk-8-jre-headless
  - cd server
  - screen -S mcs
- **(4) 2026**: *(Subsequent updates mostly focused on feature additions and bug fixes. For detailed changes, please refer to #dev-log)*
  - **1. February**:
    - ① Ver 1.1.0 (Since I couldn't find the Randman plugin (which relies on WorldBorder) back in July 2025, I had to generate random coordinates in 'the World' and use the Multiverse-Portals plugin to link 'the Lobby' to those coordinates to simulate random teleportation.)
    - ② Ver 1.1.1
  - **2. March**: Ver 1.2.0
  - **3. April**: Ver 1.2.1
  - **4. Jun 27**: Ver 1.2.2
  - **4. Jul 10**: Ver 1.2.3

### IV. Dev-log
- **Ver 0.0.0 | Jul - Aug 2024**
  - Downloaded CraftBukkit #1060 core (GitHub) and IC2, BC Bukkit backport (https://www.mcarchive.com).
- **Ver 1.0.0 | Aug 2, 2025**
  - 1. Started open beta
- **Ver 1.1.0 | February, 2026**
  - 1. Changed the Lobby. (Link: https://www.planetminecraft.com/project/castle-38/)
  - 2.I managed to find WorldGuard for Bukkit #1060 on https://www.archive.org, allowing me to protect specific regions within a world rather than locking down the whole map.So I combined the Lobby with the World.
  - 3. Created a new world named "Skyland".Added new gameplay mechanics.
  - 4. Added Randman (Based on Worldborder) plugin for random world teleportation.
- **Ver 1.1.1 | February, 2026**
  - 1. Fixed a NoSuchMethodError triggered by snow melting
  - 2. Fixed an issue preventing OP from entering the Nether.
- **Ver 1.2.0 | March 2026**
  - 1. Removed 'the Skyland'.
  - 2. Added the iConomy and ChestShop plugins and built a shop.
  - 3. Creating a Residence plot now costs money.
- **Ver 1.2.1 | April 2026**
  - 1. Adjusted a WorldBorder configuration setting (timer-delay-ticks:) to achieve true random teleportation.
  - 2. Updated shop inventory.
- **Ver 1.2.2 | June 27, 2026**
  - 1. Installed two mods: IC2 Thermometer Port & Iron Chests Port.
- **Ver 1.2.3 | July 10, 2026**
  - 1. Removed Multiverse and fixed the Nether access issues.

### V. Community
All modified plugin configurations are available in the #opensource channel on our Discord server.

If you encounter any bugs or have feedback while playing, please open an issue in this repository.
Discord:https://discord.gg/8urjC42jE3

Thank YOOOOU!!

---

<a name="chinese"></a>
## 中文

### 一、废话
当你看到这个项目时，我已经卸载了 QQ 和 discord，并把电脑上所有与学习无关的资源，剪贴到了一个硬盘上，交给父亲保管。今天是 Aug 9, 2026，距离高考还有不到 10 个月的时间 (Jun. 5, 2027)。时间过得真快。我的高中生活很快就要结束了，这让我很伤心 QwQ。

（For those unfamiliar with the Gaokao, you can think of it as an SAT taken by over 600,000 students, the New York Times wasn't exaggerating when it described it as 'thousands of troops crossing a single-log bridge. XD The Gaokao is immensely important to me—it not only determines whether I can get into my favorite university, but also defines the future of both myself and my family. Plus, for me, I only get one shot at this.)

想必没有必要多说它是多么的残酷和重要，我必须在接下来的10个月里暂停所有其他事情，放下一切准备高考。
我把我所有的项目都暂时存在 github 上这个项目（这是其中之一），以便高考后，也就是 Jun. 10, 2027 以后重新启动。

### 二、简介
这是一个从开发到运营历经4年，公测 1 年的 mods + plugins + minecraft beta 1.7.3 生存服。

### 三、发展时间表
*(我将把这些经历编辑成视频，并在高考结束后发布到YouTube和b站)*

- **（1）2022年**：自制了一些 beta1.7.3 整合包（见图1），并收集资源、网络和经验。这后来演变为该项目的客户端。
- **（2）2024年7月至8月**：专注于服务器端开发。从GitHub搞到 bukkit1060 core，从 mcarchive.org 下载了 bukkit 的 IC2 和 BC backport 及其前置（ModLoaderMP，Forge for bukkit）。将 Mods 安装到core并成功启动。（但是server core不接受任何配置文件控制。删除 META-INF 会崩溃，将 Mods 的 .zip 文件放入 mods 文件夹也会报错，——core真的就像一个jar，油盐不进。）
- **（3）2025年**：
  - **1. 7月**：
    - ① 分析服务器所需的插件（图2），并从 bukkit.org 搞到它们。研究每个作者留下的guides，并调试各个插件。
    - ② 为 IC2 安装了几个移植版附属模组。（版本1.0.0）
    - （由于当时没有找到worldguard for bukkit1060插件,而permission插件只能通过禁用一个权限组的build权限实现整个世界方块禁止破坏，所以为保护大厅，只能将主世界和大厅分成the World和the Lobby）
  - **2. 8月2日**：公测。
  - (我租用了一个云服务器 (OS is Ubuntu)，用 Xshell 连接它"那时以为 SSH 就像 Windows 的远程桌面一样，是专门进行远程访问的。但后来我在研究词典笔 (YDP031, OS is Android) (图3) 时，发现 SSH 还能连接本地的 OS。这让我明白 SSH 其实是一个控制 OS 的工具，任何 OS 都可以用它访问。（用“Shell”形容它太形象了 XD）这为我日后研究 iOS 降级提供了帮助。)
  - Ubuntu commands:
  - sudo apt update
  - sudo apt install openjdk-8-jre-headless
  - cd server
  - screen -S mcs
- **（4）2026年**：*(往后基本都是添加一些新东西和修bugs,所以就不多叙述了，详细内容看dev-log)*
  - **1. 2月**：
    - ① 1.1.0版（(由于2025年七月时没有找到Randman插件(前置Worldborder),所以只能通过随机生成一些the World的坐标，并用插件Multiverse-Portals将the Lobby与这些坐标锚定的方式实现伪随机传送。）
    - ② 版本1.1.1
  - **2. 3月**：1.2.0版
  - **3. 4月**：1.2.1版
  - **4. 6月27日**：1.2.2版

### 四、Dev-log
- **Ver 0.0.0 | 2024年7月-8月**
  - 设置 CraftBukkit #1060 核心（GitHub）和 IC2、BC Bukkit 移植版（MCArchive.com）。
- **1.0.0版 | 2025年8月2日**
  - 1. 开始开放测试版
- **Ver 1.1.0 | 2026年2月**
  - 1. 更改大厅。（链接：https://www.planetminecraft.com/project/castle-38/）
  - 2. 在https://www.archive.org找到了worldguard for bukkit1060插件，可以实现对一个世界部分区域的保护，因此将大厅与主世界合并。
  - 3. 创造了一个名为“Skyland”的新世界，增添玩法 。
  - 4. 增加了 Randman（基于 WorldBorder）插件，用于随机世界传送。
- **Ver 1.1.1 | 2026年2月**
  - 1. 修复了融雪触发的 NoSuchMethodError
  - 2. 修复了一个阻止 OP 进入下界（Nether）的问题。
- **1.2.0版 | 2026年3月**
  - 1. 移除the Skyland
  - 2. 添加了 iConomy 和 ChestShop 插件，并建立了一个商店。
  - 3. 创建 Residence 领地地块现在需要花钱。
- **1.2.1版 | 2026年4月**
  - 1. 调整了 WorldBorder 配置设置（timer-delay-ticks:），以实现真正的随机传送。
  - 2. 增添了商店的内容
- **1.2.2版 | 2026年6月27日**
  - 1. 安装了两个 Mod：IC2 Thermometer Port 和 Iron Chests Port。
- **Ver 1.2.3**
  - 1. 删除了 Multiverse 并修复了下界（Nether）访问问题。

### 五、社区
所有修改后的插件配置都可以在 Discord 服务器上的 #opensource 频道中获得。

如果您在玩游戏时遇到任何 Bug 或有反馈，请在此仓库中打开 Issue。
Discord:https://discord.gg/8urjC42jE3
QQ:316834843


谢谢你！！

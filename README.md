Status: Frozen until Jun 2027
(The server will remain up and running during this period)
这个服务器仍然运行，你可以随时进来

[English](#english) | [中文](#chinese)

---

<a name="english"></a>
## English

### I. Foreword
By the time you see this project, I will have already uninstalled QQ and Discord, transferred all non-study-related files on my computer to an external hard drive, and handed it over to my parents for safekeeping. Today is August 9, 2026, with less than 10 months to go before the Gaokao (June 2027). Time is flying by so fast—my high school days are coming to an end soon QwQ.

*(For those unfamiliar with the Gaokao, you can think of it as an SAT taken by over 10 million students nationwide. The New York Times wasn't exaggerating when describing it as "thousands of troops crossing a single-log bridge". The Gaokao is immensely important to me—it not only determines my university admission, but also defines the future path for myself and my family. Plus, I only get one shot at this.)*

There is no need to elaborate further on its importance, which is why I must put everything else on hold for the next 10 months to focus entirely on preparation. I have pushed all my projects (including this one) to GitHub so I can pick them right back up after June 10, 2027.

### II. Introduction
This repository contains the configuration, optimization logs, and custom setup for a **Minecraft Beta 1.7.3** modded server with custom Bukkit plugins and backported mods.

### III. Development Timeline
*(I will edit these experiences into a dev-log documentary and post it to YouTube after the Gaokao.)*

* **2022**: Built custom modpacks for Beta 1.7.3, gathered resources, networking setup, and technical experience. This served as the client foundation for the project.
* **July – August 2024**: Focused on server-side setup. Sourced the `CraftBukkit #1060` core from GitHub, downloaded Bukkit backports for IC2 and BuildCraft along with their prerequisites (`ModLoaderMP`, `Forge for Bukkit`) from MCArchive. Integrated mods into the core and successfully launched it.
  * *Technical Hurdle*: The vanilla Bukkit core was resistant to direct modification. Deleting `META-INF` or putting mod `.zip` files directly into `/mods` threw severe errors—it acted like a completely locked-down JAR until properly patched with Forge/ModLoaderMP dependencies.
* **July – August 2025**:
  * *July*: Analyzed required plugins via BukkitDev, debugged dependency issues, and installed several backported IC2 add-ons.
  * *August 2*: Official Open Beta release (**Ver 1.0.0**).
* **February – June 2026**: Continuous feature iterations, bug fixes, and environment stabilization (see Changelog below).

### IV. Dev-Log & Changelog

* **Ver 0.0.0** | *Jul – Aug 2024*
  * Configured `CraftBukkit #1060` core with IC2 & BuildCraft Bukkit backports.
* **Ver 1.0.0** | *Aug 2, 2025*
  * Launched Open Beta.
* **Ver 1.1.0** | *Feb 2026*
  * Redesigned Lobby architecture (Credit: [PMC Castle 38](https://www.planetminecraft.com/project/castle-38/)).
  * Merged Lobby into the main survival world.
  * Created a custom dimension world "Skyland".
  * Integrated `Randman` (WorldBorder-based) plugin for random wild teleportation.
* **Ver 1.1.1** | *Feb 2026*
  * Fixed a `NoSuchMethodError` triggered by snow melting mechanics.
  * Fixed an issue preventing OP players from entering the Nether.
* **Ver 1.2.0** | *Mar 2026*
  * Deprecated and removed "Skyland".
  * Integrated `iConomy` plugin and constructed server shop.
  * Set a currency cost for creating `Residence` claims.
* **Ver 1.2.1** | *Apr 2026*
  * Adjusted WorldBorder `timer-delay-ticks` configuration to achieve true random teleportation.
  * Updated server shop inventory and pricing.
* **Ver 1.2.2** | *Jun 27, 2026*
  * Installed backported mods: `IC2 Thermometer Port` & `Iron Chests Port`.
* **Ver 1.2.3** | *Aug 2026*
  * Removed `Multiverse-Core` dependency to resolve underlying Nether transit bugs.

### V. Community & Resources
* All modified plugin configuration files, Linux/Ubuntu deployment scripts, and server parameters are archived in the `#opensource` channel on our Discord server.
* If you encounter any bugs or have technical feedback while inspecting these configs, please feel free to **open an Issue** in this repository.
* Discord:https://discord.gg/8urjC42jE3

*Thank YOOOOU!! See you all in June 2027!*

---

<a name="chinese"></a>
## 中文
(机翻)
### 一、 写在前面
当你看到这个项目时，我已经卸载了 QQ 和 Discord，将电脑上所有与学习无关的文件转存到了移动硬盘，并交由父母妥善保管。今天是 2026 年 8 月 9 日，距离 2027 年 6 月的高考还有不到 10 个月的时间。时间飞逝，高中生活即将迎来尾声 QwQ。

高考对我而言至关重要——它不仅决定了我能否进入理想的大学，也关乎我与家庭的未来发展。对我来说，这是一场只有一次机会的硬仗。

无须多言它的关键性，因此在接下来的 10 个月里，我必须暂停一切娱乐与技术折腾，全情投入备考。我已将包括本项目在内的所有开源内容推送到 GitHub 存档，以便在 2027 年 6 月 10 日高考结束后重新解冻并继续开发。

### 二、 项目简介
本项目为一个基于 **Minecraft Beta 1.7.3** 的硬核 Mod/插件混合服务端架构存档，包含自定义 Bukkit 插件调试、老版本 Mod Backport（逆向移植）及底层性能优化配置。

### 三、 开发时间线
*(高考结束后，我计划将这段时间的开发经历剪辑成一部纪录片/开发日志发布到 YouTube。)*

* **2022 年**：制作 Beta 1.7.3 客户端整合包，积累资源、网络配置及技术经验，为本项目客户端奠定基础。
* **2024 年 7 月 – 8 月**：专注于服务端核心构建。从 GitHub 获取 `CraftBukkit #1060` 核心，并从 MCArchive 匹配 IC2、BuildCraft 的 Bukkit Backport 版本及其前置（`ModLoaderMP`、`Forge for Bukkit`）。成功完成 Mod 与核心的整合并启动。
  * *技术踩坑*：原始 Bukkit 核心对外部修改非常敏感，直接删除 `META-INF` 或将 Mod 压缩包放入 `/mods` 文件夹均会抛出严重异常，必须通过正确的 Forge/ModLoaderMP 依赖层进行修补。
* **2025 年 7 月 – 8 月**：
  * *7 月*：筛选 Bukkit 插件，排查依赖冲突，完成各插件的单独调试与 IC2 扩展移植。
  * *8 月 2 日*：服务器正式开启 Open Beta 测试（**Ver 1.0.0**）。
* **2026 年 2 月 – 6 月**：持续进行功能迭代、底层 Bug 修复与配置优化（详见下方更新日志）。

### 四、 开发日志 (Dev-Log)

* **Ver 0.0.0** | *2024年7月 – 8月*
  * 构建 `CraftBukkit #1060` 核心及 IC2、BuildCraft 移植版环境。
* **Ver 1.0.0** | *2025年8月2日*
  * 开启 Open Beta 公测。
* **Ver 1.1.0** | *2026年2月*
  * 更换主城架构（主城建筑参考：[PMC Castle 38](https://www.planetminecraft.com/project/castle-38/)）。
  * 将主城世界与主生存世界进行无缝合并。
  * 新建“Skyland（天空之城）”自定义维度。
  * 引入基于 WorldBorder 的 `Randman` 随机传送插件。
* **Ver 1.1.1** | *2026年2月*
  * 修复积雪融化时抛出的 `NoSuchMethodError` 异常。
  * 修复 OP 权限玩家无法正常进入地狱（Nether）的 Bug。
* **Ver 1.2.0** | *2026年3月*
  * 移除“Skyland”维度以简化架构。
  * 引入 `iConomy` 经济系统并搭建服务器商店。
  * 设定 `Residence` 领地创建消耗游戏币。
* **Ver 1.2.1** | *2026年4月*
  * 调整 WorldBorder 的 `timer-delay-ticks` 配置参数，实现真正的无卡顿随机传送。
  * 更新商店售卖物品列表及定价。
* **Ver 1.2.2** | *2026年6月27日*
  * 移植并安装两大 Mod：`IC2 Thermometer Port` 与 `Iron Chests Port`（更多箱子）。
* **Ver 1.2.3** | *2026年8月*
  * 移除 `Multiverse-Core` 多世界插件，彻底解决地狱传送门响应异常问题。

### 五、 社区与资源
* 所有修改后的插件配置文件、Ubuntu 部署脚本及运维参数均已归档至 Discord 服务器的 `#opensource` 频道。
* 若您在参考或使用相关配置时遇到任何技术 Bug，欢迎在此 GitHub 存储库中提交 **Issue**。
* * Discord:https://discord.gg/8urjC42jE3
  * QQ:316834843

*非常感谢大家！2027 年 6 月，我们高处相见！*

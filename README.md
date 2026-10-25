# Minecraft 全版本下载器

一键下载 Minecraft **全部 1120 个版本**（正式版 / 快照 / Beta / 远古版 / **愚人节版本** / **未发布版本** / **其他特别版**），支持**官方源**和**国内镜像**，自动打包为 ZIP。

🔗 **在线使用**：https://lindedaoqwq.github.io/minecraft-downloader/

---

## 快速开始

1. **打开网页**：https://lindedaoqwq.github.io/minecraft-downloader/
2. **找到版本**：在列表里翻找，或直接用搜索框搜索（如 `1.7.10`、`combat test 7`、`战斗测试`）；点上方「愚人节」「未发布」「其他特别版」标签可只看特别版本
3. **点击「ZIP」按钮**：在版本行的右侧
4. **选择下载源**：
   - 🟩 **官方源** —— Mojang 官方服务器，最权威
   - 🟪 **存档源（Omniarchive）** —— Omniarchive 社区档案（仅 Omniarchive 独家版本）
   - 🟦 **BMCLAPI 镜像** —— 国内加速通道，下载更快
5. **等待打包完成**，浏览器会自动开始下载

> 想下载服务端？点开版本详情，选择「客户端 / 服务端」后再选下载源即可。

## 特别版本：愚人节 & 未发布 & 其他特别版

除了官方启动器列出的 920 个版本，本站还收录了官方清单之外的特别版本（数据整理自社区项目 [zkitefly/unlisted-versions-of-minecraft](https://github.com/zkitefly/unlisted-versions-of-minecraft) 与 [Omniarchive](https://omniarchive.net) 社区档案）：

| 分类 | 收录内容 |
|---|---|
| 🎭 愚人节（13 个） | 2.0（蓝/红/紫/预览版）、15w14a、1.RV-Pre1、3D Shareware v1.34、20w14∞、22w13oneBlockAtATime、23w13a_or_b、24w14potato、25w14craftmine、26w14a |
| 🔒 未发布（22 个） | **Combat Test 1–8c 全系列 12 个**（1.14_combat-212796 = CT 1、1.14_combat-0 = CT 2、1.14_combat-3 = CT 3、1.15_combat-1 = CT 4、1.15_combat-6 = CT 5、1.16_combat-0 = CT 6、1.16_combat-1/-2/-3 = CT 7/7b/7c、1.16_combat-4/-5/-6 = CT 8/8b/8c；其中 7 / 7b / 8 为私有测试版）、1.18 / 1.19 实验快照、Beta 1.2_02 开发者版（20110517）、MINECON 2011 展示版（1.0.0-tominecon）等 |
| 🧩 其他特别版（3 个） | Minecraft 4K（4k-1 / 4k-2）、PC Gamer 演示版（b1.3-pcgamer） |
| 📜 远古未列出（171 个） | 官方清单之外的 11w–13w 快照、Alpha / Beta 零散版本 |

> 愚人节版本分类依据 [Minecraft Wiki](https://minecraft.wiki/w/Java_Edition_versions#April_Fools'_versions)。注意 20w14a / 22w13a / 23w13a / 24w14a 是愚人节当周发布的**常规快照**（Wiki 有消歧义说明），不属于愚人节版本；15w14a 与 26w14a 为真正的愚人节版本。

> **Omniarchive 独家版本**：2.0-preview（2013 年私下发给 YouTuber 的 2.0 预览版）、1.0.0-tominecon（MINECON 2011 展示版）、b1.2_02-20110517（开发者版）、b1.3-pcgamer（PC Gamer 杂志 214 期 DVD 演示版）、4k-1 / 4k-2（2009 年 Java 4K 竞赛作品）原版均无官方 JSON 发布，其 JSON 为社区整理元数据（详情页已注明），JAR 由 [vault.omniarchive.uk](https://vault.omniarchive.uk) 存档分发。

## ZIP 里有什么

每个 ZIP 包含两个文件：

| 文件 | 说明 |
|---|---|
| `版本号.json` | Mojang 官方版本元数据**原文**（一个字节都没有改动；Omniarchive 独家版本为社区整理元数据，详情页已注明） |
| `版本号.jar` | 游戏文件（客户端或服务端，与官方文件完全一致，SHA1 校验相同；Omniarchive 独家版本由社区档案分发） |

## 常见问题

**官方源和 BMCLAPI 下载的文件有区别吗？**
没有。两个源的文件字节完全一致（SHA1 相同），BMCLAPI 只是国内加速通道，文件实际由 Mojang 官方服务器分发。

**为什么有些版本没有服务端？**
Mojang 官方早期版本未发布服务端文件，这种情况下「服务端」选项会置灰，无法选择。

**愚人节 / 未发布版本为什么只有官方源？**
这些版本不在 Mojang 官方清单内，BMCLAPI 只镜像官方清单，因此仅提供官方源（文件同样来自 Mojang 服务器，或 Omniarchive 等社区镜像存档）。

**打包过程能看到进度吗？**
可以。进度面板上有进度条和终端风格的控制台日志，显示每个阶段的详细情况；随时可以点「取消」中止。

**版本列表会过期吗？**
不会。版本数据自动检测自 Mojang 官方版本清单，新版本发布后打开网页即可看到。

**手机能用吗？**
可以。页面已针对手机屏幕优化，下载按钮和弹窗均适配触屏操作。

## 版本类型说明

| 类型 | 含义 |
|---|---|
| 正式版 | 稳定发布的游戏版本 |
| 快照 | 测试中的预览版本 |
| 实验版 | 未正式发布的实验性版本（Combat Test / 实验快照） |
| Beta | 2010-2011 年的 Beta 测试版 |
| 远古版 | 更早的 Alpha/Classic 等经典版本 |
| 特别版 | Omniarchive 独家特别版本（Minecraft 4K，独立于常规版本线） |

---

*本项目为第三方工具，与 Mojang / Microsoft 无关联。游戏文件版权归 Mojang 所有。*

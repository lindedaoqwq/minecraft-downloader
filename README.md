# Minecraft 全版本下载器

一个纯前端实现的 Minecraft 全版本下载网页：自动检测 Mojang 官方版本清单中的**全部 920 个版本**（正式版 / 快照 / Beta / 远古版），点击下载时可选**官方源**或 **BMCLAPI 镜像**，并将文件打包为 ZIP（官方版本 JSON + JAR）后由浏览器直接下载。

## 功能特性

- **自动检测全部版本**：数据来自 Mojang 官方版本清单 `launchermeta.mojang.com`，无需手动维护版本列表
- **双下载源**：官方源（Mojang 权威来源）/ BMCLAPI 国内镜像，每次下载时弹窗选择
- **ZIP 打包**：内含 `{版本号}.json`（Mojang 官方版本元数据**原文**，字节未做任何改动）与 `{版本号}.jar`（与官方文件 SHA1 一致），不含其他文件
- **打包过程可视化**：进度条 + 终端风格控制台日志，支持随时取消
- **液态玻璃 UI**：参考 Prisma Minecraft iOS Launcher 设计风格，移动端优先适配
- **零依赖**：单 HTML 文件，手写 ZIP 生成器（store 模式 + CRC32），无任何外部 JS/CSS 框架

## 在线使用

部署后访问：`https://<你的用户名>.github.io/minecraft-downloader/`

## 本地使用

直接用浏览器打开 `index.html` 即可；或启动一个静态服务器：

```bash
python3 -m http.server 8000
# 访问 http://localhost:8000
```

## 数据来源

| 内容 | 来源 |
|---|---|
| 版本清单 | `https://launchermeta.mojang.com/mc/game/version_manifest.json` |
| 版本 JSON（ZIP 内） | 清单内 `version.url`（piston-mojang.com 官方原文） |
| JAR 文件 | 官方 `downloads.{client,server}.url`（piston-data / launcher.mojang.com） |
| BMCLAPI 镜像 | `https://bmclapi2.bangbang93.com`（302 至 piston-data 同 hash 对象） |

## 说明

- ZIP 内的 JSON 为 Mojang 官方版本元数据原文，与官方启动器下载的文件字节级一致
- BMCLAPI 镜像的文件字节实际由 `piston-data.mojang.com` 分发，与其直链下载完全一致
- 本项目为第三方工具，与 Mojang / Microsoft 无关联

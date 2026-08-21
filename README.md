# Connector Suite Public Releases

Connector Suite 是一个本地 Agent 与 WPS/Office 之间的统一连接器。

本仓库是**公开分发仓库**，只提供安装包、SHA-256 校验文件、版本说明和更新清单；
Connector Suite 源代码、模块实现和构建工程保留在私有仓库中，不在此仓库公开。

## 当前版本

- 版本：`0.2.1-dev`
- 渠道：开发测试版
- macOS：`Connector-Suite-Installer-0.2.1-dev.dmg`
- Windows：`Connector-Suite-Installer-0.2.1-windows-dev.zip`

这是开发测试版，不代表稳定发布。安装前请确认目标电脑已经安装兼容的 WPS/Office 和
Node.js 运行环境，并保留安装日志和报告。

## 安装

### macOS

1. 下载 Release 中的 DMG。
2. 挂载 DMG，运行 `Install Connector Suite.command`。
3. 按提示完成证书授权、运行时安装和宿主加载项配置。
4. 安装器只有在健康检查、加载项和在线 session 门禁通过时才会报告成功。

### Windows

1. 下载 Release 中的 ZIP。
2. 解压到本地可写目录。
3. 运行 `Install Connector Suite.cmd`。
4. 按安装报告检查 Platform、Office、WPS、证书、manifest、计划任务和 session 状态。

## 完整性校验

下载后请根据 `checksums/` 中对应的 SHA-256 文件校验安装包。校验不一致时不要运行安装器。

## 更新清单

机器可读清单：[`update-manifest.json`](./update-manifest.json)

## 许可与源码

本仓库只负责公开分发，不授予 Connector Suite 源码、构建系统或内部实现的使用许可。
产品源码仓库保持私有。

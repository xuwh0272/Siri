# Siri AI & Dynamic Island for Windows

Windows 桌面上的 Siri AI 助手与灵动岛个人实验项目，探索玻璃质感界面、动态交互与桌面体验。

## 下载与安装

**[前往 Releases 下载安装版](https://github.com/xuwh0272/Siri/releases)**

在 Releases 的 **Assets** 中下载 `Siri-DynamicIsland-Setup-0.1.0-beta.1-win-x64.exe`，双击安装。安装包包含 Siri AI、灵动岛、玻璃效果辅助程序、Inter 字体及应用专用 .NET 8 桌面运行环境，提供桌面、开始菜单和卸载入口。默认不启用开机启动。

也可以下载 `Siri-DynamicIsland-0.1.0-beta.1-win-x64.zip`，解压后运行 `Launcher.exe`。不要只把启动器复制出来，程序需要压缩包内的其他文件。

系统要求：Windows 10 2004 或更新版本、Windows 11，x64。Siri 还使用 Windows 自带的 .NET Framework 4.8 与系统语音。当前为未代码签名的 Beta 版本，Windows 可能显示未知发布者。

## 首次使用

- 从桌面或开始菜单启动两个程序；也可从开始菜单分别启动。
- 按住 Esc 约 0.6 秒唤起 Siri，短按 Esc 关闭。
- **AI 模型不包含在安装包中**。需要自行运行本地 OpenAI-compatible 模型服务，并编辑安装目录中的 `SiriAI/config/local-model.txt`。默认模板地址为 `http://127.0.0.1:11434/v1`，模型为 `gemma3:4b`，应填写实际可用的模型 ID。模型服务未配置时，AI 问答不可用。
- 未打包离线神经语音模型，保留系统语音备用。详细说明见包内 `使用说明.txt`。
- 卸载可使用 Windows“设置 → 应用”或开始菜单中的卸载入口；使用后产生的数据和配置会保留。

## 持续更新

本项目将持续更新，逐步改进功能、界面动画、Siri 与灵动岛联动、兼容性和稳定性。进展以提交记录和 Releases 为准，具体功能与发布时间以实际发布为准。欢迎通过 Issues 反馈问题和建议。

## 源码与验证范围

安装版对应源码见 Release 附件 `Siri-DynamicIsland-Source-0.1.0-beta.1.zip`；其中也包含安装器与启动器源码。仓库原有 `Siri-source.zip` 是首次公开时的源码快照。

本次在本机检查了安装解包、文件完整性、内置 .NET 环境、灵动岛程序入口和 Siri 静态渲染。不同电脑上的完整交互、AI 模型连接及所有外设功能仍需持续验证。

## 非官方项目声明

这是个人独立开发与实验项目，与 Apple Inc. 无隶属、授权、赞助或官方合作关系，不是 Apple 官方产品，不提供 Apple 官方 Siri 服务。Siri、Dynamic Island（灵动岛）、Apple 等名称及相关商标属于各自权利人。

第三方代码、依赖、字体、图标和其他素材的权利及许可证归原作者所有。Inter 字体许可和运行环境许可随安装包提供。仓库公开不代表所有内容均获准再分发或商业使用；在完成来源核对前，暂不对整个项目统一授予开源许可。详见 [NOTICE.md](NOTICE.md)。

安装包不包含作者的私人对话、账号令牌或私人 AI 配置。请勿在 Issues 或公开日志中提交密钥和私人内容。

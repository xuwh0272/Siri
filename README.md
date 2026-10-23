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
- **AI 模型不包含在安装包中**。需要自行运行本地 Google Gemma 模型服务，并编辑安装目录中的 `SiriAI/config/local-model.txt`。默认模板地址为 `http://127.0.0.1:11434/v1`，模型为 `gemma3:4b`，应填写实际可用的模型 ID。模型服务未配置时，AI 问答不可用。

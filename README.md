# YouTube 工作台下载

[下载 v0.7.0 独立安装版](https://github.com/waltertech/youtube-workbench-releases/releases/tag/v0.7.0)

系统要求：**Apple Silicon（M 系列）Mac，macOS 26 或更新版本**。暂不提供 Intel Mac 或 Windows 安装包。

## 安装

下载 `YouTube-Workbench-0.7.0-macOS-arm64.dmg`，将「YouTube 工作台」拖入 Applications 后启动。

安装包内置 Python、FFmpeg、NumPy、Codex CLI、OCR 与封面组件，无需开发项目、Homebrew 或 Xcode。首次启动自动检测组件并准备本机工作空间。AI 功能需自行登录 Codex 或配置相应服务，离线制作不要求登录。

此包尚未完成 Apple Developer ID 签名与公证；首次打开若被 macOS 拦截，需要用户在系统「隐私与安全性」中确认来源。已通过隔离 HOME/PATH、只读 DMG 运行验证，但未在另一台物理新 Mac 上测试。

## 更新

右上角下载图标或「本机设置 → 检查更新」，弹框显示更新内容、下载进度，支持取消和重试。下载完毕校验 SHA256，点击「打开安装包」安装。替换应用前结束任务并退出旧版本。

用户数据和素材位于应用外；旧开发版用户可在首次检测页面选择「沿用旧版工作空间」，指向原来的 `.runtime` 目录，保留历史记录。

## 发布附件

- DMG：独立应用安装包。
- SHA256SUMS：下载完整性校验，不等同于 Apple 签名。
- YouTubeWorkbench-corresponding-sources.tar.gz：随附 FFmpeg 等开源组件的对应源码、构建配方及许可证；应用内另含第三方声明。

本仓库仅公开分发安装产物。工作台业务源码与开发交接保存在私有仓库。

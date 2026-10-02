# Changelog / 更新日志

All notable changes to Anulus are documented here. This project follows
[Semantic Versioning](https://semver.org/) and the spirit of
[Keep a Changelog](https://keepachangelog.com/).

本文件记录 Anulus 的重要变更，遵循语义化版本规范。
分类含义：**Added** 新增 · **Changed** 变更 · **Fixed** 修复 · **Removed** 移除 · **Security** 安全。

---

## [Unreleased] / 未发布

Work in progress before the first public release. 首个公开版本发布前的进行中工作。

### Fixed / 修复
- Stability and defect fixes ahead of the first public build. 首个公开版本前的稳定性与缺陷修复。

---

## [3.1.1] - not yet released / 尚未发布

> First public release. Fill this section in when the installer is final, then move it above the
> `Unreleased` block and tag the repository.
> 首个公开版本。安装包定稿后补全本节，将其置于 `Unreleased` 之上，并为仓库打标签。

### Added / 新增
- Local-first AI assistant: works with cloud providers you configure, or with a fully on-device engine.
  本地优先的 AI 助手：可接自行配置的云端服务，或使用完全离线的设备端引擎。
- Office toolset: documents, tables, notes and text utilities the assistant can operate directly.
  办公工具集：文档、表格、笔记与文本工具，助手可直接操作。
- On-device image editor with filters, layout and export.
  设备端图片编辑器，含滤镜、排版与导出。
- File manager, project boards and date-organised working files.
  文件管理、项目看板与按日期组织的工作文件。
- Plugin system with two package formats: `.axext` (plain) and `.axex` (encrypted).
  插件体系，两种插件包格式：`.axext`（明文）与 `.axex`（加密）。
- Voice input, scanning, floating-ball quick access and small games.
  语音输入、扫码、悬浮球快捷入口与小游戏。

### Security / 安全
- Local HTTP service bound to the loopback address only. 本机 HTTP 服务仅监听回环地址。
- Release builds are code-shrunk and obfuscated. 发布版本启用代码压缩与混淆。

### Known limitations / 已知限制
- `arm64-v8a` devices only. 仅支持 `arm64-v8a` 设备。
- The fully offline engine needs a capable device and separately downloaded model files.
  完全离线引擎需要性能足够的设备，并单独下载模型文件。

---

<!--
Template for future entries / 后续版本条目模板

## [X.Y.Z] - YYYY-MM-DD
Installer: Anulus-X.Y.Z-arm64-v8a.apk
SHA-256: <checksum>

### Added / 新增
### Changed / 变更
### Fixed / 修复
### Security / 安全
-->

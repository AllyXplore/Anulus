# Third-Party Notices / 第三方组件声明

Anulus is proprietary software that builds on open-source work. This file lists the third-party
components distributed with, or used by, the application, together with their licences. Each component
remains governed by its own licence, which takes precedence over the Anulus
[end-user licence](LICENSE.md) for that component.

Anulus 为闭源软件，但建立在众多开源工作之上。本文件列出随应用分发或被应用使用的第三方组件及其许可证。
每个组件仍受其自身许可证约束；对该组件而言，其许可证优先于 Anulus 的[最终用户许可协议](LICENSE.md)。

Copies of the licence texts are included in the application package and are also shown in the app under
**About → Open-source and third-party components**.
许可证文本随应用包提供，也可在应用内 **关于 → 开源与第三方组件** 中查看。

If you believe a component is missing or misattributed, please open an issue — corrections are welcome.
如发现遗漏或标注有误，欢迎提交问题反馈，我们会更正。

---

## Model inference and engines / 模型推理与引擎

| Component | Purpose | Licence |
| --- | --- | --- |
| llama.cpp (ggerganov) | GGUF model inference engine / 模型推理引擎 | MIT |
| whisper.cpp (ggerganov) | Speech recognition engine / 语音识别引擎 | MIT |
| Hugging Face | Model hosting and distribution / 模型托管与分发 | Apache-2.0 |
| Vosk (alphacep) | Offline speech recognition / 离线语音识别 | Apache-2.0 |

## Runtime and frameworks / 运行时与框架

| Component | Purpose | Licence |
| --- | --- | --- |
| Tauri | Cross-platform application framework / 跨平台应用框架 | MIT OR Apache-2.0 |
| tauri-plugin-opener | System opener plugin / 系统打开器插件 | MIT OR Apache-2.0 |
| Chaquopy (chaquo) | Python runtime for Android / 安卓 Python 运行时 | MIT |
| serde, serde_json, tokio, futures-util | Rust ecosystem / Rust 生态基础库 | MIT OR Apache-2.0 |

## Front-end and interface / 前端与界面

| Component | Purpose | Licence |
| --- | --- | --- |
| Tailwind CSS | Styling framework / 样式框架 | MIT |
| CodeMirror | Code editor / 代码编辑器 | MIT |
| KaTeX | Math rendering / 数学公式渲染 | MIT |
| marked.js | Markdown parsing / Markdown 解析 | MIT |
| Mermaid | Diagram rendering / 流程图与图表渲染 | MIT |
| Three.js | 3D rendering / 3D 渲染 | MIT |
| Font Awesome | Icons / 图标 | MIT (icons: CC BY 4.0) |
| html2canvas | Page capture and export / 页面截图与导出 | MIT |
| DOMPurify | HTML sanitisation / HTML 内容净化 | MPL-2.0 (also Apache-2.0) |
| JSZip | Archiving / 压缩与打包 | MIT |
| QRCode | QR code generation / 二维码生成 | MIT |

## Rust crates (backend) / 后端与系统库

| Component | Purpose | Licence |
| --- | --- | --- |
| image | Image encode/decode and processing / 图片编解码与处理 | MIT OR Apache-2.0 |
| zip | ZIP archives / ZIP 压缩 | MIT |
| base64 | Encoding / 编码 | MIT OR Apache-2.0 |
| aes, aes-gcm, cbc, cipher, des, pbkdf2 | Cryptography / 加解密套件 | MIT OR Apache-2.0 |
| md-5, sha1, sha2, digest | Hashing / 哈希套件 | MIT OR Apache-2.0 |
| serde_yaml | YAML parsing / YAML 解析 | MIT OR Apache-2.0 |
| pulldown-cmark | Markdown to HTML / Markdown 转 HTML | MIT |
| regex, scraper, url | Text and HTML parsing / 文本与 HTML 解析 | MIT OR Apache-2.0 |
| kamadak-exif | Image EXIF reading / 图片 EXIF 读取 | MIT |
| reqwest | HTTP client / HTTP 客户端 | MIT OR Apache-2.0 |
| tiny_http | Local HTTP micro-service / 本地 HTTP 微服务 | MIT OR Apache-2.0 |
| tar, flate2 | Compression / 压缩 | MIT OR Apache-2.0 |
| ed25519-compact | Author signature verification / 作者签名验签 | MIT OR Apache-2.0 |
| uuid, rand, hex, urlencoding, html-escape | Utilities / 通用工具 | MIT OR Apache-2.0 |

## Android native components / 安卓原生组件

| Component | Purpose | Licence |
| --- | --- | --- |
| AndroidX WebKit | WebView support / WebView 支持 | Apache-2.0 |
| AndroidX AppCompat | Backward-compatible UI / 向后兼容界面 | Apache-2.0 |
| AndroidX Activity KTX | Activity extensions / Activity 扩展 | Apache-2.0 |
| AndroidX Lifecycle | Lifecycle management / 生命周期管理 | Apache-2.0 |
| Material Design Components (Google) | UI components / 界面控件 | Apache-2.0 |

---

## Notes---

## Notes on specific licences / 关于特定许可证

- **MPL-2.0 (DOMPurify).** The component is used in unmodified form. Its source is publicly available
  from the upstream project; if you need the exact version shipped in a given release, open an issue and
  we will point you to it.
  该组件按原样使用，未作修改。其源码可从上游项目公开获取；如需某个发行版实际内置的具体版本，
  可提交问题反馈，我们会指明。
- **Apache-2.0 components.** Required notices are retained in the application package.
  Apache-2.0 组件所需的声明文件已随应用包保留。
- **Font Awesome.** Icon artwork is used under CC BY 4.0; the accompanying code is MIT.
  图标素材依 CC BY 4.0 使用，配套代码为 MIT。

Trade names and logos of third parties are the property of their respective owners and are used here only
to identify the corresponding components.
第三方名称与标识归其各自所有者所有，此处仅用于标识对应组件。




# Frequently Asked Questions / 常见问题

[English](#english) · [简体中文](#简体中文)

---

## English

**Is Anulus free?**
Yes. The app is free to download and use. Paid value-added features may appear later; if they do, they will be optional
and clearly marked.

**What language is the interface in?**
The interface is currently Simplified Chinese. An English interface is planned but not shipped yet — the
documentation in this repository is bilingual so that international users can evaluate the app before
installing. If you rely on an English UI, watch the repository for that milestone.

**Does it need an internet connection?**
Not for the core tools, the image editor, the file manager or the on-device engine. You need a connection
for: cloud AI providers you configure, downloading models, the in-app browser.

**Which AI providers does it work with?**
Providers you configure yourself, using your own credentials and endpoint. Nothing is pre-filled with our
keys, and we do not resell model access. Alternatively, run a model fully on the device.

**Can it really run AI offline?**
Yes, through the on-device engine plugin. You download a model file once, then inference runs locally with
no network. Speed and quality depend on your device and the model size; 6 GB of RAM or more is recommended.

**Where is my data stored? Is there a cloud backup?**
Everything is local: app storage plus the `Anulus` folder in shared storage. There is no cloud backup,
because there is no server. Copy the `Anulus` folder to a computer if you want a backup.

**Why is it not on Google Play or a Chinese app store?**
Store listings are a separate process with their own requirements. Direct distribution from a versioned
release page with published checksums is the current approach. That is also why your device will warn about
an "unknown developer" — see [INSTALL.md](INSTALL.md).

**Is the source code available?**
No. Anulus is proprietary software maintained by a very small team; publishing the source is not part of
the plan. Third-party open-source components are credited in
[../THIRD-PARTY-NOTICES.md](../THIRD-PARTY-NOTICES.md).

**Why does it declare so many permissions?**
Because it bundles many tools. Each sensitive permission is requested only when you use the feature behind
it, and refusing simply disables that feature. Full breakdown:
[PERMISSIONS.md](PERMISSIONS.md).


**What are `.axext` and `.axex` plugins? Where do I get them?**
They are the two Anulus plugin package formats — plain and encrypted. They are equal formats, not
different products. There is no third-party plugin marketplace at launch; install only packages from
authors you trust.

**Is there an iOS, desktop or tablet version?**
Android phones are the target today. The app runs on Android tablets but the layout is tuned for phones.
No iOS build.

**Does it work on a rooted device?**
Usually, but it is not tested against custom system modifications. Root also weakens the isolation the app
relies on, so treat that as your own risk.

**How do I update?**
Install the newer version over the old one; do not uninstall first. Watch the release page, or use the
watch/star function on the repository to be notified.

**I found a bug. Where do I report it?**
[../SUPPORT.md](../SUPPORT.md) explains what to include. Security problems go through
[../SECURITY.md](../SECURITY.md) instead of a public issue.

---

## 简体中文

**Anulus 收费吗？**
免费下载使用。后续可能出现付费增值功能，
如果有，会是可选的，并明确标注。

**界面是什么语言？**
目前界面为简体中文。英文界面在计划中，尚未发布——本仓库文档做成中英双语，是为了让国际用户在安装前
就能了解应用。如果你必须用英文界面，请关注仓库的相关进展。

**必须联网吗？**
核心工具、图片编辑器、文件管理器和设备端引擎都不需要联网。需要联网的是：
你自行配置的云端 AI 服务、模型下载、应用内浏览器。

**支持哪些 AI 服务？**
支持你自己配置的服务，使用你自己的凭据和接口地址。我们不预置任何密钥，也不转卖模型额度。
你也可以完全在设备上跑模型。

**真的能离线跑 AI 吗？**
可以，通过设备端引擎插件。模型文件下载一次之后，推理全程在本地进行，不需要网络。
速度和效果取决于设备性能与模型大小，建议 6 GB 及以上运行内存。

**数据存在哪里？有云端备份吗？**
全部在本地：应用私有存储，加上共享存储里的 `Anulus` 文件夹。没有云端备份，因为没有服务器。
需要备份就把 `Anulus` 文件夹拷到电脑上。

**为什么不上应用商店？**
上架是另一套流程，有各自的要求。目前采取的方式是从带版本号的发行版页面直接分发，并公布校验值。
这也是设备会提示“开发者未知”的原因，见 [INSTALL.md](INSTALL.md)。

**开源吗？**
不开源。Anulus 是由极小团队维护的闭源软件，公开源码不在计划内。
所用第三方开源组件在 [../THIRD-PARTY-NOTICES.md](../THIRD-PARTY-NOTICES.md) 中致谢。

**为什么声明了这么多权限？**
因为它内置了很多工具。每项敏感权限只在你使用对应功能时申请，拒绝也只是让该功能不可用。
逐项说明见 [PERMISSIONS.md](PERMISSIONS.md)。




**`.axext` 和 `.axex` 插件是什么？在哪里获取？**
它们是 Anulus 的两种插件包格式——明文与加密，地位平等，不是两种不同产品。
首发不开放第三方插件市场，请只安装你信任的作者提供的插件包。

**有 iOS、电脑或平板版本吗？**
目前面向安卓手机。安卓平板可以运行，但界面按手机布局调优。没有 iOS 版本。

**已获取超级用户权限（root）的设备能用吗？**
通常可以，但未针对各种系统改造做测试。这类环境也会削弱应用依赖的隔离机制，风险请自行判断。

**怎么升级？**
用新版本直接覆盖安装，不要先卸载。关注发行版页面，或用仓库的关注功能接收通知。

**发现问题去哪里反馈？**
[../SUPPORT.md](../SUPPORT.md) 说明了需要提供的信息。
安全问题请走 [../SECURITY.md](../SECURITY.md)，不要公开提交。





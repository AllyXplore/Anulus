# Privacy Policy / 隐私政策

**Application:** Anulus (`com.allyxplore.anulus`) · **Publisher:** AllyXplore
**Last updated:** 2026-08-19

> English first, Chinese below. 英文在前，中文在后。两个版本如有歧义，以中文版本为准。

---

## English

### Summary

Anulus is designed local-first. There is no Anulus server: we operate no backend, we hold no user
accounts, and we receive none of your content. Your data lives on your device. The only outbound network
traffic the app initiates on your behalf goes to endpoints **you** configure.

| We do not | Notes |
| --- | --- |
| Require an account | Core features work fully offline |
| Collect analytics or usage telemetry | No product analytics component is embedded |
| Upload your chats, files, notes or images | They never leave the device unless you send or export them |
| Operate a server that stores your data | There is no such server |

### 1. Information we collect

The core features run locally on your device, including the local backend service and, optionally,
on-device model inference. When you are not using a feature that requires the network, we do not collect,
store or upload your personal information.

For anti-fraud, service integrity and statistical accuracy, we may in future obtain device and network
information comparable to that described in section 6 (device model, system version, coarse region).
No such collection is enabled today; if it is enabled later, this policy will be updated first.

### 2. Data storage

Most of your data — conversations, preferences, on-device models, plugin data, entitlement flags — is
stored in your device's local storage: the app's own cache, date-organised working files, and the
`Anulus` folder visible in your file manager.

Uninstalling the app, clearing its data, or resetting the device **permanently deletes** this data. Keep
your own backups. (There is currently no paid membership system; the entitlement field is reserved for
possible future value-added services.)

### 3. AI services you configure

The AI assistant requires either your own third-party credentials (for example a cloud model provider)
or a local inference engine.

If you use a cloud provider, the text you submit is transmitted directly from your device to the endpoint
you entered, to generate a reply. We are not an intermediary, we do not proxy or log those requests, and
we are not responsible for the third party's data practices. Please avoid entering sensitive personal
information in prompts.

### 4. Permissions

The app requests system permissions only to deliver specific features, and uses each one only while the
corresponding feature is running. A permission-by-permission table — what it is for, and what happens if
you deny it — is in [docs/PERMISSIONS.md](docs/PERMISSIONS.md).

If you grant a permission to a third-party plugin, please evaluate it carefully. How a plugin uses
permissions is the responsibility of its author.

### 5. Local network service

The app runs a small HTTP service on the device, bound to the loopback address (`localhost`) only. It is
used for communication between the app's own modules — for example, the floating-ball overlay calling
local AI capabilities. It does not send your data outside the device and is not reachable from other
devices on your network.

### 6. Data security

We apply reasonable technical measures to protect your local data, but no measure is unbreakable. We are
not liable for leakage or loss caused by device loss, system failure, malware or similar causes outside
our control.

### 7. Children

The app is not directed at persons under 18. Minors should use it under the guidance of a parent or
guardian.

### 8. International users

Because the app has no backend of ours, we perform no cross-border transfer of your data. Any transfer
that occurs is between your device and the third-party endpoint you chose, governed by their own policies. Mandatory rights you hold under your local law
are unaffected.

### 9. Changes

We may update this policy. The updated version takes effect when published in the app or in this
repository. Continued use indicates acceptance.

### 10. Contact

Community channel: https://pd.qq.com/qqweb/qunpro/share?_wv=3&_wwv=128&appChannel=share&attaContentID=7824cc8ef7d54615a238e9f4ee7f38eb&biz=ka&businessType=5&from=246611&inviteCode=2LWrRnNgUhY&mainSourceId=qr_code&subSourceId=pic4&b=5 · Security reports: see [SECURITY.md](SECURITY.md)

The software is provided as is. We do not promise technical support or a customer-service response time;
see [SUPPORT.md](SUPPORT.md).

---

## 简体中文

### 摘要

Anulus 以本地优先为设计原则。我们没有 Anulus 服务器：不运营后端、不持有用户账号、也拿不到你的任何内容。
你的数据存在你的设备上。应用代你发起的对外网络请求，只会发往**你自己配置的**接口。

| 我们不会 | 说明 |
| --- | --- |
| 要求注册账号 | 核心功能可完全离线使用 |
| 采集使用统计 | 未内置产品分析组件 |
| 上传你的对话、文件、笔记、图片 | 除你主动发送或导出，它们不离开设备 |
| 运营存放你数据的服务器 | 不存在这样的服务器 |

### 一、信息收集

核心功能在你的设备本地运行（含本地后端服务与可选的本地模型推理）。在你未主动使用需联网的功能时，
我们不会收集、存储或上传你的个人信息。

为防范作弊、保障服务安全与统计准确性，我们未来可能获取与第 6 条相类似的设备与网络信息
（设备型号、系统版本、粗略地区等）。目前尚未启用此类采集，如后续启用，将先更新本政策说明。

### 二、数据存储

你的大部分数据（聊天记录、设置偏好、本地模型与插件数据、权益状态等）保存在设备本地存储中：
应用自身缓存、按日期组织的文件，以及文件管理中可见的 `Anulus` 文件夹。

卸载应用、清除数据或恢复出厂设置将**永久删除**这些数据，请自行备份。
（当前尚无会员体系，“权益状态”仅为后续增值服务预留的数据字段。）

### 三、你配置的 AI 服务

AI 助手需要你自行提供第三方凭据（例如某家云端模型服务）或使用本地推理引擎。

若使用云端服务，你提交的文本会从你的设备直接传输至你填写的接口用于生成回复。
我们不作中转、不代理、不记录这些请求，也不对第三方的数据处理行为负责。建议不要在提问中输入个人敏感信息。

### 四、权限

应用仅为实现具体功能申请系统权限，且只在对应功能运行时使用。逐项权限说明（用途，以及拒绝后的影响）
见 [docs/PERMISSIONS.md](docs/PERMISSIONS.md)。

若你向第三方插件授予权限，请谨慎评估。插件如何使用权限由其作者负责。

### 五、本机网络服务

应用在设备上运行一个小型 HTTP 服务，仅监听本机回环地址（`localhost`），
用于应用内部模块之间的通信（例如悬浮球调用本地 AI 能力）。它不会把你的数据发往设备外部，
同一网络中的其他设备也无法访问。

### 六、数据安全

我们采取合理的技术手段保护你的本地数据，但没有任何安全措施是绝对不可破解的。
对于因设备丢失、系统故障、恶意软件等我们无法控制的原因导致的泄露或丢失，我们不承担责任。

### 七、未成年人

本软件不面向 18 周岁以下人士。未成年人应在监护人指导下使用。

### 八、国际用户

由于我们没有自有后端，我们不进行你数据的跨境传输。发生的传输只存在于你的设备与你选择的第三方接口之间，
受其各自政策约束。你依所在地法律享有的强制性权利不受影响。

### 九、政策变更

我们可能更新本政策，更新版本在软件内或本仓库公布后生效，你继续使用即表示接受。

### 十、联系方式

社区频道：https://pd.qq.com/qqweb/qunpro/share?_wv=3&_wwv=128&appChannel=share&attaContentID=7824cc8ef7d54615a238e9f4ee7f38eb&biz=ka&businessType=5&from=246611&inviteCode=2LWrRnNgUhY&mainSourceId=qr_code&subSourceId=pic4&b=5 · 安全问题反馈：见 [SECURITY.md](SECURITY.md)

本软件按现状提供，我们不承诺技术支持或客服响应时限，详见 [SUPPORT.md](SUPPORT.md)。



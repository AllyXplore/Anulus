# Permissions / 权限说明

[English](#english) · [简体中文](#简体中文)

This page lists every permission declared by Anulus, why it exists, and what happens if you refuse it.
Nothing here is used for profiling or content upload.

本页列出 Anulus 声明的全部权限、存在的原因，以及拒绝后的影响。
这些权限都不用于画像或内容上传。

---

## English

### How permissions are requested

- Sensitive permissions are requested **at the moment a feature needs them**, not at first launch.
- Declining is always allowed. The related feature stays unavailable; the rest of the app works.
- A permission you granted can be revoked at any time in Android settings.
- Third-party plugins run inside the app. If a plugin asks you to grant something, judge the plugin, not
  the app — plugin behaviour is the plugin author's responsibility.

### Always-on, non-sensitive

| Permission | Why |
| --- | --- |
| `INTERNET` | Cloud AI providers you configure, model downloads, the in-app browser |
| `VIBRATE` | Haptic feedback |
| `WAKE_LOCK` | Keeps long jobs alive: local inference, large downloads |
| `FOREGROUND_SERVICE` (+ `DATA_SYNC`, `SPECIAL_USE`) | Runs the local engine, downloads and the floating ball as a visible foreground service instead of a hidden background one |
| `POST_NOTIFICATIONS` | Task progress and reminders you asked for |
| `SCHEDULE_EXACT_ALARM` | Reminders that must fire at a precise time |
| `RECEIVE_BOOT_COMPLETED` | Restores your scheduled reminders after a reboot |
| `REQUEST_IGNORE_BATTERY_OPTIMIZATIONS` | Optional prompt, so aggressive power saving does not kill a running local job |
| `SYSTEM_ALERT_WINDOW` | The floating-ball quick-access overlay |
| `QUERY_ALL_PACKAGES` | Lets "open with" / "share to" list the apps installed on your device |
| `INSTALL_SHORTCUT` | Creates home-screen shortcuts when you ask for one |

### Requested on demand, sensitive

| Permission | Why | If you deny |
| --- | --- | --- |
| `CAMERA` | Taking photos, scanning codes | Camera-based tools unavailable |
| `RECORD_AUDIO` | Voice input, recording transcription | Voice features unavailable |
| `READ_MEDIA_IMAGES` / `VIDEO` / `AUDIO` | Opening your media in the image editor and attaching files | You can still use files picked through the system picker |
| `READ_EXTERNAL_STORAGE` (Android 12L and older) | Reading files on older systems | File features limited on those systems |
| `MANAGE_EXTERNAL_STORAGE` | The built-in file manager, and reading or writing the shared `Anulus` folder across the whole storage. This is a broad permission — it is requested only if you use the file manager, and it is never used to scan your storage for analytics | File manager unavailable; other features keep working through the system picker |
| `ACCESS_COARSE_LOCATION` | Region-level features | Location-aware tools unavailable |
| `ACCESS_FINE_LOCATION` | Tools that need your precise position when you invoke them | Those tools unavailable |
| `READ_CONTACTS` | Assistant tools that look up a contact when you ask them to | Those tools unavailable |
| `READ_CALENDAR` | Assistant tools that read your schedule when you ask them to | Those tools unavailable |
| `READ_SMS` / `SEND_SMS` | Message-related assistant tools, invoked explicitly by you | Those tools unavailable |
| `READ_PHONE_STATE` | Device state checks used by hardware-dependent features | Those features unavailable |
| `BODY_SENSORS` | Health-sensor readings for wearable-linked features | Those features unavailable |
| `BLUETOOTH_CONNECT` / `BLUETOOTH_SCAN` / `NEARBY_WIFI_DEVICES` | Pairing with wearables and other devices for cross-device control | Cross-device features unavailable |

### What is never done

- No upload of your conversations, notes, files or images to us — we run no server.
- No background collection of contacts, messages, calendar entries or location.
- No use of the sensitive permissions above for profiling.
- No hidden audio or camera capture: capture happens only while the corresponding feature is on screen.

If a build ever behaves otherwise, treat it as a security issue and report it — see
[../SECURITY.md](../SECURITY.md).

---

## 简体中文

### 权限申请方式

- 敏感权限**在具体功能需要时**才申请，不在首次启动时一次性索取。
- 你随时可以拒绝。对应功能保持不可用，应用其余部分照常使用。
- 已授予的权限可随时在系统设置中收回。
- 第三方插件运行在应用内部。若插件要求你授予某项权限，请评估该插件本身——插件行为由其作者负责。

### 常驻且不敏感的权限

| 权限 | 用途 |
| --- | --- |
| `INTERNET` 网络 | 你自行配置的云端 AI 服务、模型下载、应用内浏览器 |
| `VIBRATE` 振动 | 触感反馈 |
| `WAKE_LOCK` 保持唤醒 | 让长任务不被中断：本地推理、大文件下载 |
| `FOREGROUND_SERVICE`（含 `DATA_SYNC`、`SPECIAL_USE`） | 以可见的前台服务运行本地引擎、下载与悬浮球，而不是隐藏的后台进程 |
| `POST_NOTIFICATIONS` 通知 | 任务进度与你设置的提醒 |
| `SCHEDULE_EXACT_ALARM` 精准定时 | 需要按精确时间触发的提醒 |
| `RECEIVE_BOOT_COMPLETED` 开机启动 | 重启后恢复你设置的定时提醒 |
| `REQUEST_IGNORE_BATTERY_OPTIMIZATIONS` 忽略电池优化 | 可选提示，避免激进省电策略杀掉正在运行的本地任务 |
| `SYSTEM_ALERT_WINDOW` 悬浮窗 | 悬浮球快捷入口 |
| `QUERY_ALL_PACKAGES` 查询已安装应用 | 让“用其他应用打开”“分享到”能列出你设备上的应用 |
| `INSTALL_SHORTCUT` 创建快捷方式 | 在你要求时创建桌面快捷方式 |

### 按需申请的敏感权限

| 权限 | 用途 | 拒绝后 |
| --- | --- | --- |
| `CAMERA` 相机 | 拍照、扫码 | 相机相关工具不可用 |
| `RECORD_AUDIO` 麦克风 | 语音输入、录音转写 | 语音功能不可用 |
| `READ_MEDIA_IMAGES` / `VIDEO` / `AUDIO` 媒体读取 | 在图片编辑器中打开你的媒体文件、添加附件 | 仍可通过系统选择器挑选文件使用 |
| `READ_EXTERNAL_STORAGE`（安卓 12L 及更早） | 在旧系统上读取文件 | 这些系统上的文件功能受限 |
| `MANAGE_EXTERNAL_STORAGE` 所有文件访问 | 内置文件管理器，以及在整个存储范围读写共享的 `Anulus` 文件夹。这是范围很大的权限——仅在你使用文件管理器时申请，且绝不用于扫描你的存储做统计 | 文件管理器不可用，其余功能仍可通过系统选择器工作 |
| `ACCESS_COARSE_LOCATION` 粗略位置 | 地区级功能 | 位置相关工具不可用 |
| `ACCESS_FINE_LOCATION` 精确位置 | 你主动调用的、需要精确位置的工具 | 这些工具不可用 |
| `READ_CONTACTS` 通讯录 | 你要求助手查找联系人时使用 | 相关工具不可用 |
| `READ_CALENDAR` 日历 | 你要求助手读取日程时使用 | 相关工具不可用 |
| `READ_SMS` / `SEND_SMS` 短信 | 与消息相关的助手工具，由你明确触发 | 相关工具不可用 |
| `READ_PHONE_STATE` 设备状态 | 依赖硬件状态的功能所需的检查 | 相关功能不可用 |
| `BODY_SENSORS` 身体传感器 | 与可穿戴设备联动的健康数据读取 | 相关功能不可用 |
| `BLUETOOTH_CONNECT` / `BLUETOOTH_SCAN` / `NEARBY_WIFI_DEVICES` | 与手环等设备配对，实现跨设备控制 | 跨设备功能不可用 |

### 我们绝不会做的事

- 不把你的对话、笔记、文件或图片上传给我们——我们没有服务器。
- 不在后台采集通讯录、短信、日历或位置。
- 不把上述敏感权限用于用户画像。
- 不做隐蔽的录音或拍摄：采集只发生在对应功能处于前台使用时。

若某个版本表现与此不符，请按安全问题处理并反馈，见 [../SECURITY.md](../SECURITY.md)。




# Installation Guide / 安装指南

[English](#english) · [简体中文](#简体中文)

---

## English

### 1. Check your device

| Requirement | Value |
| --- | --- |
| Android version | 7.0 (API 24) or newer |
| CPU architecture | `arm64-v8a` (64-bit ARM) |
| Free storage | about 120 MB for the app |
| RAM for the offline engine | 6 GB or more recommended |

Not sure about the architecture? Almost every phone sold since 2018 is `arm64-v8a`. If installation fails
with "package appears to be invalid" on a very old or budget device, it is likely 32-bit and unsupported.

### 2. Download the installer

Get it from the official page:

- GitHub: https://github.com/AllyXplore/Anulus/releases/latest


Download the file named `Anulus-<version>-arm64-v8a.apk`.

### 3. Verify the download (recommended)

Compare the SHA-256 checksum and signing fingerprint published on the release page with your file.
Full instructions: [VERIFY.md](VERIFY.md). This is the only reliable way to know the file was not
tampered with in transit.

### 4. Allow installation from your source

Android blocks installers from unknown sources by default. Grant permission to the app you are installing
*from* (your browser or file manager):

- **Stock Android / Pixel:** tap the downloaded file, then **Settings** in the prompt, and enable
  *Allow from this source*.
- **Samsung One UI:** Settings → Apps → your browser → **Install unknown apps** → allow.
- **Xiaomi HyperOS / MIUI:** allow the install prompt; if a security scan warning appears, choose
  *Install anyway*. Some regions also require turning off *Settings → Privacy protection → Special
  permissions → Install unknown apps* restrictions for your browser.
- **HUAWEI EMUI / HarmonyOS:** if *Pure mode* (纯净模式) is on, disable it in
  Settings → Security → More settings → Pure mode, then install.
- **OPPO ColorOS / OnePlus / realme:** confirm the *Install blocked* dialog, then allow the source.
- **vivo OriginOS / Funtouch:** Settings → More settings → Permission management → Install unknown apps.

You may see a Google Play Protect warning about an unrecognised developer. That warning appears for every
app distributed outside the Play Store; choose to install anyway if you have verified the checksum.

### 5. Install and open

Tap the file, confirm, and wait for it to finish. Open Anulus from your app drawer.

### 6. First run

The app asks for permissions only when a feature needs one. You can decline anything you do not want; the
related feature simply stays unavailable. See [PERMISSIONS.md](PERMISSIONS.md) for what each permission
does.

If you plan to use the fully offline AI engine, download the model file from inside the app: open the
engine plugin and pick a model. Models are large — use Wi-Fi and expect several gigabytes for larger ones.

### 7. Updating

Install the new version over the old one. Do **not** uninstall first: uninstalling deletes your local
data, and there is no cloud backup.

Downgrading is not supported. Android refuses to install an older version over a newer one; you would have
to uninstall (losing data) first.

### 8. Uninstalling

Uninstall as usual. Your conversations, notes and settings are removed with the app. The `Anulus` folder
in shared storage may remain — delete it manually if you want a clean removal.

### Troubleshooting

| Symptom | Likely cause and fix |
| --- | --- |
| "App not installed" / "package appears invalid" | Incomplete download, or a 32-bit device. Re-download and check the checksum. |
| "App not installed as package conflicts with an existing package" | A build with a different signature is already installed. Uninstall it first (this deletes its data). |
| Installation blocked with no explanation | Pure mode / security scan on the device skin. See step 4. |
| Installer downloads as `.apk.html` or `.bin` | Your browser renamed it. Rename back to `.apk`, or download with a different browser. |
| App opens then closes immediately | Report it with your device model and system version — see [../SUPPORT.md](../SUPPORT.md). |

---

## 简体中文

### 一、确认设备

| 要求 | 数值 |
| --- | --- |
| 系统版本 | 安卓 7.0（接口级别 24）及以上 |
| 处理器架构 | `arm64-v8a`（64 位 ARM） |
| 可用空间 | 应用本身约 120 MB |
| 离线引擎所需运行内存 | 建议 6 GB 及以上 |

不确定架构？2018 年之后上市的手机几乎都是 `arm64-v8a`。若在很旧或很低端的机型上提示“安装包无效”，
大概率是 32 位设备，不受支持。

### 二、下载安装包

只从官方页面获取：

- GitHub：https://github.com/AllyXplore/Anulus/releases/latest


下载名为 `Anulus-<版本号>-arm64-v8a.apk` 的文件。

### 三、校验下载（建议执行）

把发行版页面公布的 SHA-256 校验值与签名指纹跟你下载的文件比对，方法见 [VERIFY.md](VERIFY.md)。
这是判断文件在传输途中是否被替换的唯一可靠方式。

### 四、允许来自该来源的安装

安卓默认拦截未知来源的安装包。需要给“执行安装的那个应用”（浏览器或文件管理器）授权：

- **原生安卓 / Pixel：** 点开安装包，在提示里进入**设置**，开启“允许来自此来源”。
- **三星 One UI：** 设置 → 应用 → 你的浏览器 → **安装未知应用** → 允许。
- **小米 HyperOS / MIUI：** 在安装提示中允许；若出现安全扫描风险提示，选择“继续安装”。
  部分地区还需在 设置 → 隐私保护 → 特殊权限 → 安装未知应用 中为浏览器解除限制。
- **华为 EMUI / HarmonyOS：** 若开启了**纯净模式**，先在 设置 → 安全 → 更多安全设置 → 纯净模式 中关闭，再安装。
- **OPPO ColorOS / 一加 / 真我：** 在“已阻止安装”对话框中确认，然后允许该来源。
- **vivo OriginOS / Funtouch：** 设置 → 更多设置 → 权限管理 → 安装未知应用。

可能出现谷歌 Play 保护机制关于“开发者未知”的提示。所有不经应用商店分发的应用都会触发该提示；
若你已核对过校验值，可选择继续安装。

### 五、安装并打开

点击文件，确认安装，等待完成，然后在桌面或应用列表中打开 Anulus。

### 六、首次使用

应用只在具体功能需要时才申请权限。你可以拒绝任何不想给的权限，对应功能保持不可用即可，
各项权限用途见 [PERMISSIONS.md](PERMISSIONS.md)。

若打算使用完全离线的 AI 引擎，请在应用内下载模型：打开引擎插件并选择模型。
模型文件体积较大，建议在无线网络下下载，较大的模型可能需要数 GB 空间。

### 七、升级

直接覆盖安装新版本。**不要**先卸载：卸载会删除本地数据，且没有云端备份。

不支持降级。安卓不允许用旧版本覆盖新版本，只能先卸载（会丢数据）再装。

### 八、卸载

按常规方式卸载即可。聊天记录、笔记与设置会随应用一并删除。
共享存储中的 `Anulus` 文件夹可能保留，如需彻底清除请手动删除。

### 常见故障

| 现象 | 可能原因与处理 |
| --- | --- |
| 提示“应用未安装”“安装包无效” | 下载不完整，或设备是 32 位。重新下载并核对校验值。 |
| 提示“与现有应用签名冲突” | 设备上已装了签名不同的版本。先卸载它（会删除其数据）。 |
| 无提示直接被拦截 | 系统的纯净模式或安全扫描所致，见第四步。 |
| 下载得到 `.apk.html` 或 `.bin` | 浏览器改了后缀。改回 `.apk`，或换个浏览器下载。 |
| 打开后立刻退出 | 请附设备型号与系统版本反馈，见 [../SUPPORT.md](../SUPPORT.md)。 |

# Verify Your Download / 校验你下载的安装包

[English](#english) · [简体中文](#简体中文)

---

## English

### Why bother

An installer distributed outside an app store can be modified by whoever hosts or relays it. Two values
let you detect that:

1. the **SHA-256 checksum** — proves the file is byte-for-byte the one we published;
2. the **signing certificate fingerprint** — proves the app was signed with our key, and that any future
   update comes from the same source.

Every release page lists both. If either does not match, do not install the file.

### Official signing fingerprint

| Field | Value |
| --- | --- |
| Package name | `com.allyxplore.anulus` |
| Certificate SHA-256 | `57:6D:0B:4E:C9:E0:09:2D:6F:AB:55:76:55:11:20:06:12:98:9E:33:1F:42:34:86:8F:25:73:A3:D4:AD:94:EE` |

This fingerprint stays the same for every official release. It never changes, so you can save it once and
compare it later. A file whose fingerprint differs is **not** an official build, whatever its version
number says.

### Check the checksum on a computer

**Windows (Command Prompt)**

```
certutil -hashfile "C:\path\to\Anulus-3.1.4-arm64-v8a.apk" SHA256
```

**Windows (PowerShell)**

```
Get-FileHash -Algorithm SHA256 "C:\path\to\Anulus-3.1.4-arm64-v8a.apk"
```

**macOS**

```
shasum -a 256 ~/Downloads/Anulus-3.1.4-arm64-v8a.apk
```

**Linux**

```
sha256sum ~/Downloads/Anulus-3.1.4-arm64-v8a.apk
```

Compare the output with the checksum on the release page. Case and spacing do not matter; the hex digits
must be identical.

### Check the checksum on the phone itself

Any file manager with a "file details" or "hash" function will do. With Termux installed:

```
sha256sum /sdcard/Download/Anulus-3.1.4-arm64-v8a.apk
```

### Check the signing fingerprint

With the Android SDK build tools on a computer:

```
apksigner verify --print-certs "C:\path\to\Anulus-3.1.4-arm64-v8a.apk"
```

Look for the line reporting the **certificate SHA-256 digest** and compare it with the table above.

Alternative without the SDK: use any app that displays the signature of an installed application, then
compare the SHA-256 fingerprint it shows for `com.allyxplore.anulus`.

### If something does not match

- Re-download from the official page — an interrupted download is the most common cause.
- If it still does not match, the file is not the one we published. Delete it and report where you got it,
  through the channels in [../SECURITY.md](../SECURITY.md).

---

## 简体中文

### 为什么要校验

不经应用商店分发的安装包，可能被托管方或中转方修改。两个值可以让你发现这种情况：

1. **SHA-256 校验值**——证明文件和我们发布的完全一致（逐字节相同）；
2. **签名证书指纹**——证明应用由我们的密钥签名，也保证后续更新来自同一来源。

每个发行版页面都会公布这两项。任一不一致，就不要安装该文件。

### 官方签名指纹

| 项目 | 值 |
| --- | --- |
| 应用包名 | `com.allyxplore.anulus` |
| 证书 SHA-256 指纹 | `57:6D:0B:4E:C9:E0:09:2D:6F:AB:55:76:55:11:20:06:12:98:9E:33:1F:42:34:86:8F:25:73:A3:D4:AD:94:EE` |

该指纹在所有官方版本中保持不变，可以保存下来长期比对。
指纹不同的文件**不是**官方版本，无论它标着什么版本号。

### 在电脑上核对校验值

**Windows（命令提示符）**

```
certutil -hashfile "C:\路径\Anulus-3.1.4-arm64-v8a.apk" SHA256
```

**Windows（PowerShell）**

```
Get-FileHash -Algorithm SHA256 "C:\路径\Anulus-3.1.4-arm64-v8a.apk"
```

**macOS**

```
shasum -a 256 ~/Downloads/Anulus-3.1.4-arm64-v8a.apk
```

**Linux**

```
sha256sum ~/Downloads/Anulus-3.1.4-arm64-v8a.apk
```

把输出与发行版页面上的校验值比对。大小写和空格无关，十六进制数字必须完全相同。

### 直接在手机上核对

任何带“文件详情”或“哈希值”功能的文件管理器都可以。若装有 Termux：

```
sha256sum /sdcard/Download/Anulus-3.1.4-arm64-v8a.apk
```

### 核对签名指纹

在装有安卓开发工具的电脑上：

```
apksigner verify --print-certs "C:\路径\Anulus-3.1.4-arm64-v8a.apk"
```

找到输出中报告**证书 SHA-256 摘要**的那一行，与上面的表格比对。

没有开发工具时的替代方式：用任意可查看已安装应用签名信息的工具，
对照它显示的 `com.allyxplore.anulus` 的 SHA-256 指纹。

### 如果对不上

- 先从官方页面重新下载——下载中断是最常见的原因。
- 若仍然对不上，说明该文件不是我们发布的版本。请删除它，并通过
  [../SECURITY.md](../SECURITY.md) 中的渠道告知我们它的来源。

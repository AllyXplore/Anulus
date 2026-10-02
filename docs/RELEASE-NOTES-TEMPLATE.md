# Release notes template / 发行说明模板

Copy everything between the two rulers into the release description box, then replace the placeholders.
把两条分隔线之间的内容整段复制到发行版说明框里，然后替换占位内容。

Placeholders to replace / 需要替换的占位：
`<VERSION>` version number 版本号 · `<DATE>` release date 发布日期 · `<SHA256>` checksum 校验值 ·
`<SIZE>` file size 文件大小

---

## Anulus <VERSION>

**Release date / 发布日期:** <DATE>
**Platform / 平台:** Android 7.0+ · `arm64-v8a` only

### Download / 下载

| File | Size | SHA-256 |
| --- | --- | --- |
| `Anulus-<VERSION>-arm64-v8a.apk` | <SIZE> | `<SHA256>` |

Signing certificate SHA-256 / 签名证书 SHA-256:
`57:6D:0B:4E:C9:E0:09:2D:6F:AB:55:76:55:11:20:06:12:98:9E:33:1F:42:34:86:8F:25:73:A3:D4:AD:94:EE`

Please verify before installing / 安装前请先校验: [docs/VERIFY.md](../docs/VERIFY.md)
Installation guide / 安装指南: [docs/INSTALL.md](../docs/INSTALL.md)

### What's new / 更新内容

**Added / 新增**
- ...

**Changed / 变更**
- ...

**Fixed / 修复**
- ...

**Security / 安全**
- ...

### Upgrade notes / 升级说明

- Install over the previous version. Do not uninstall first — uninstalling deletes local data.
  直接覆盖安装，不要先卸载——卸载会删除本地数据。
- Downgrading is not supported. 不支持降级。

### Known issues / 已知问题

- ...

### Notes / 说明

- Interface language is Simplified Chinese; bilingual documentation is in the repository.
  界面语言为简体中文，仓库内提供中英双语文档。
- No account required. No analytics. Your content stays on the device.
  无需账号，无使用统计，内容保留在设备本地。
- Third-party plugins are the responsibility of their authors.
  第三方插件由其作者负责。
- Full history / 完整历史: [CHANGELOG.md](../CHANGELOG.md) ·
  Privacy / 隐私: [PRIVACY.md](../PRIVACY.md) ·
  Licence / 许可: [LICENSE.md](../LICENSE.md)

---

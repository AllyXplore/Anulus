# Security Policy / 安全政策

## Supported versions / 支持的版本

Only the latest published release receives fixes. Older installers are kept for reference only.
仅最新发布版本会获得修复，旧安装包仅作留存参考。

| Version / 版本 | Supported / 是否支持 |
| --- | --- |
| Latest release / 最新发布版 | Yes / 是 |
| Earlier releases / 更早版本 | No / 否 |

## Reporting a vulnerability / 报告安全问题

Please **do not** open a public issue for a security problem. Report it privately first:
请**不要**为安全问题公开提交 issue，先通过私下渠道报告：

1. Preferred — GitHub private vulnerability reporting: use the **Security → Report a vulnerability**
   button on this repository.
   首选——GitHub 私密漏洞报告：使用本仓库的 **Security → Report a vulnerability** 入口。
2. Alternative — send a private message to the maintainer in the community channel:
   https://pd.qq.com/qqweb/qunpro/share?_wv=3&_wwv=128&appChannel=share&attaContentID=7824cc8ef7d54615a238e9f4ee7f38eb&biz=ka&businessType=5&from=246611&inviteCode=2LWrRnNgUhY&mainSourceId=qr_code&subSourceId=pic4&b=5
   备选——在社区频道私信维护者：https://pd.qq.com/qqweb/qunpro/share?_wv=3&_wwv=128&appChannel=share&attaContentID=7824cc8ef7d54615a238e9f4ee7f38eb&biz=ka&businessType=5&from=246611&inviteCode=2LWrRnNgUhY&mainSourceId=qr_code&subSourceId=pic4&b=5
3. Email (if you prefer): `385906668@qq.com`
   邮件（如你更习惯）：`385906668@qq.com`

Helpful details / 请尽量包含：

- affected version and device / 受影响版本与设备型号
- Android version / 系统版本
- what an attacker could achieve / 攻击者可以做到什么
- steps to reproduce, and a proof of concept if you have one / 复现步骤，如有验证代码请附上
- whether you want to be credited in the release notes / 是否希望在发行说明中致谢

## What to expect / 处理流程

This project is maintained by a very small team, so no response time is guaranteed. In practice:
本项目由极小的团队维护，因此不承诺响应时限。通常流程为：

1. Acknowledgement of your report. 确认收到报告。
2. Assessment and reproduction. 评估并复现。
3. A fix in the next release, with a note in [CHANGELOG.md](CHANGELOG.md) under **Security**.
   在下一个版本中修复，并在 [CHANGELOG.md](CHANGELOG.md) 的 **Security** 分类中记录。
4. Public disclosure after the fixed installer is published — please hold off until then.
   修复版安装包发布后再公开披露——在此之前请暂不公开。

We do not run a paid bug-bounty programme. Credit in the release notes is offered instead, if you want it.
本项目没有付费漏洞奖励计划，如你愿意，我们会在发行说明中致谢。

## Scope / 适用范围

In scope / 属于范围内：

- the Anulus application itself, as distributed from the official release pages
  从官方发行版页面分发的 Anulus 应用本身
- the local HTTP service, local file handling, plugin loading and permission handling
  本机 HTTP 服务、本地文件处理、插件加载与权限处理
- the installer's integrity and signing / 安装包完整性与签名

Out of scope / 不属于范围内：

- third-party plugins, and anything a plugin does after you install it
  第三方插件，以及安装后插件的行为
- third-party AI providers you configure with your own credentials
  你用自己凭据配置的第三方 AI 服务
- modified, repackaged or unofficially signed builds
  经修改、重打包或非官方签名的版本
- issues that require an already-compromised or rooted device with the attacker in physical control
  需要设备已被攻破、已获取超级用户权限，或攻击者掌握物理控制才能成立的问题

## Verifying what you installed / 确认你安装的版本

Before reporting, please confirm your installer is official by checking its checksum and signing
fingerprint: [docs/VERIFY.md](docs/VERIFY.md).
报告前请先按 [docs/VERIFY.md](docs/VERIFY.md) 核对校验值与签名指纹，确认安装包为官方版本。





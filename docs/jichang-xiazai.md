# 机场下载去哪下：项目发布页与文件核对
更新:2026-11-05 · 依据:项目发布记录与项目说明

机场下载要先找到客户端自己的项目发布页。取得安装文件后，再对照系统、芯片架构和项目提供的校验信息。

## 各客户端在哪里发布？

各项目有自己的 Releases，也就是版本及附件的发布位置。下表仓库名为文字标识，不是安装包下载直链。

截至 2026-11-05，版本与发布附件记录如下。系统列仅转述附件覆盖情况，不能替代项目的系统支持说明。

| 客户端 | 附件覆盖系统 | 发布仓库 | 版本 |
| --- | --- | --- | --- |
| Clash Verge Rev | Windows、macOS、Linux | `clash-verge-rev/clash-verge-rev` | v2.5.10 |
| FlClash | Android、Windows、macOS、Linux | `chen08209/FlClash` | v0.9.3 |
| Clash Party | Windows、macOS、Linux | `mihomo-party-org/clash-party` | v2.0.4 |
| Clash Meta for Android | Android | `MetaCubeX/ClashMetaForAndroid` | v2.11.36 |
| v2rayN | Windows、macOS、Linux | `2dust/v2rayN` | 7.25.6 |
| v2rayNG | Android | `2dust/v2rayNG` | 2.3.15 |

没有列出的系统不据名称补齐。需要选择哪款客户端，可查看仓库首页的「客户端怎么选」。

## 文件名怎样对应设备？

先看系统与架构，再区分安装版和便携版。架构是文件对应的处理器类型，与安装形式是不同条件。

- Windows 对照 x64，ARM 笔记本对照 arm64。
- `setup.exe` 是安装形式，`zip` 或 `portable` 是便携形式。
- Mac 的 Apple 芯片对应 arm64 或 aarch64。
- Android 可对照 arm64-v8a，仍需看设备架构。

文件后缀相近不能替代架构核对。系统名称相同，也还要继续读安装文件里的架构标记。

## 怎样认清项目渠道？

Clash Verge Rev 对应表中列出的项目仓库。名称相近、位置靠前，都不能代替对项目归属的核对。

截至 2026-11-05，原版 Clash 仓库接口返回 404。这个状态只对应原项目，不能代替其他客户端的发布记录。

## 下载后能核对什么？

FlClash 与 v2rayN 提供的核对信息不同。前者附带 `SHA256SUMS`，后者的发布文件带 GPG 签名。

| 项目 | 核对信息 |
| --- | --- |
| FlClash | SHA256SUMS，用于核对下载文件 |
| v2rayN | GPG 签名，项目说明还提供公钥指纹 |

SHA256SUMS 是文件校验信息。GPG 签名配合项目给出的公钥指纹核对文件，不能仅凭安装包名称判断身份。

## 相关页面

- [客户端与订阅怎样配合](https://www.jichangyyds.com/topics/clash/)
- [取得客户端后的订阅导入说明](https://www.jichangyyds.com/dingyue/)

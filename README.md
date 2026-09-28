# 梦游日本 · 桌面软件分发

[网站下载页](https://mengyouriben.com/downloads/docs/)

## 2026-09-28 首批发布

| 产品 | 当前版本 | 安装包 | Ed25519 分发元数据 | 发布记录 |
|---|---|---|---|---|
| 梦游｜媒体整理 | v0.3.2 | [下载](https://raw.githubusercontent.com/mengyouriben/mengyou-downloads/main/releases/mengyou-media-organizer/0.3.2/%E6%A2%A6%E6%B8%B8%EF%BD%9C%E5%AA%92%E4%BD%93%E6%95%B4%E7%90%86%20v0.3.2-setup.exe) | [清单](updates/mengyou-media-organizer.json) · [公钥](updates/mengyou-media-organizer.ed25519.pub) | [Release](https://github.com/mengyouriben/mengyou-downloads/releases/tag/mengyou-media-organizer-v0.3.2) |
| 梦游｜音乐播放器 | v0.1.101 | [下载](https://download.mengyouriben.com/releases/mengyou-music-player/0.1.101/%E6%A2%A6%E6%B8%B8%EF%BD%9C%E9%9F%B3%E4%B9%90%E6%92%AD%E6%94%BE%E5%99%A8-0.1.101-setup.exe) | [清单](updates/mengyou-music-player.json) · [公钥](updates/mengyou-music-player.ed25519.pub) | [Release](https://github.com/mengyouriben/mengyou-downloads/releases/tag/mengyou-music-player-v0.1.101) |
| 梦游｜截图便签 | v0.2.1 | [下载](https://raw.githubusercontent.com/mengyouriben/mengyou-downloads/main/releases/snap-note/0.2.1/%E6%A2%A6%E6%B8%B8%EF%BD%9C%E6%88%AA%E5%9B%BE%E4%BE%BF%E7%AD%BE%20v0.2.1-setup.exe) | [清单](updates/snap-note.json) · [公钥](updates/snap-note.ed25519.pub) | [Release](https://github.com/mengyouriben/mengyou-downloads/releases/tag/snap-note-v0.2.1) |
| 梦游｜电脑资源监视器 | v0.2.0 | [下载](https://raw.githubusercontent.com/mengyouriben/mengyou-downloads/main/releases/cpu-cpu-cpu-50-70/0.2.0/%E6%A2%A6%E6%B8%B8%EF%BD%9C%E7%94%B5%E8%84%91%E8%B5%84%E6%BA%90%E7%9B%91%E8%A7%86%E5%99%A8%20v0.2.0-setup.exe) | [清单](updates/cpu-cpu-cpu-50-70.json) · [公钥](updates/cpu-cpu-cpu-50-70.ed25519.pub) | [Release](https://github.com/mengyouriben/mengyou-downloads/releases/tag/cpu-cpu-cpu-50-70-v0.2.0) |
| 梦游｜知要 | v0.1.12 | [下载](https://download.mengyouriben.com/releases/personal-inbox-ledger/0.1.12/%E6%A2%A6%E6%B8%B8%EF%BD%9C%E7%9F%A5%E8%A6%81%20v0.1.12-setup.exe) | [清单](updates/personal-inbox-ledger.json) · [公钥](updates/personal-inbox-ledger.ed25519.pub) | [Release](https://github.com/mengyouriben/mengyou-downloads/releases/tag/personal-inbox-ledger-v0.1.12) |

安装包按 `releases/<product_key>/<version>/` 路径不可变保存。媒体整理、截图便签和电脑资源监视器使用本仓库 raw 路径；音乐播放器与知要使用工作室 R2 下载域名。GitHub Release 仅记版本与外链，不挂载资产。

`updates/<product_key>.json` 是带 Ed25519 签名的当前分发清单，包含安装包大小和 SHA-256；对应公开公钥是同目录的 `.ed25519.pub`。签名使用排除 `signature` 字段后的 UTF-8 JSON，键排序、无多余空格。客户端更新实现各自负责：媒体整理已接入此清单；音乐播放器的旧 RSA-PSS R2/Worker 自动更新线路迁移另定；其余三款没有程序内在线更新。

本仓库只保存已批准公开的安装包、签名清单和公开发布元数据；不保存源码、私钥、凭据或用户资料，也不承担账号与会员授权。

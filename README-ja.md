<div align="center">
  
<img src="src/assets/logo.svg" alt="logo" width="200" height="200">

# 海晶灯（Sea Lantern）

Tauri 2 + Rust + Vue 3 をベースにした、軽量な Minecraft サーバー管理ツールです。

| [![github-stars](https://img.shields.io/github/stars/SeaLantern-Studio/SeaLantern?style=flat&logo=github&label=Stars)](https://github.com/SeaLantern-Studio/SeaLantern/stargazers) | [![github-forks](https://img.shields.io/github/forks/SeaLantern-Studio/SeaLantern?style=flat&logo=github&label=Forks)](https://github.com/SeaLantern-Studio/SeaLantern/network/members) | [![github-latest](https://img.shields.io/github/v/release/SeaLantern-Studio/SeaLantern?style=flat&logo=github&label=最新バージョン)](https://github.com/SeaLantern-Studio/SeaLantern/releases/latest)                                                                                   |
| :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [![gitee-stars](https://gitee.com/fps_z/SeaLantern/badge/star.svg?theme=dark)](https://gitee.com/fps_z/SeaLantern/stargazers)                                                      | [![gitee-forks](https://gitee.com/fps_z/SeaLantern/badge/fork.svg?theme=dark)](https://gitee.com/fps_z/SeaLantern/members)                                                              | [![gitee-latest](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fgitee.com%2Fapi%2Fv5%2Frepos%2FFPS_Z%2FSeaLantern%2Freleases%2Flatest&query=%24.tag_name&label=最新バージョン&color=brightgreen&logo=gitee&style=flat)](https://gitee.com/FPS_Z/SeaLantern/releases/latest) |

<kbd>[简体中文](README.md)</kbd> <kbd>[English](README-en.md)</kbd> <kbd>日本語</kbd>


---

</div>

![img](https://gitee.com/fps_z/markdown/raw/master/img/about2.png)

## 主な機能

- **リアルタイムログ**: コンソールでログをリアルタイムに確認し、コマンドを直接入力可能。
- **GUI設定エディタ**: `server.properties` を直接編集せず、直感的な UI で設定を変更。
- **プレイヤー管理**: ホワイトリスト、BAN、OP権限をワンクリックで管理。
- **自動停止機能**: アプリ終了時にサーバーを自動で安全に停止し、データの紛失を防止。
- **アップデート確認**: 新しいバージョンを自動チェックし、ワンクリックでダウンロード。

## クイックスタート

[最新リリース](https://github.com/SeaLantern-Studio/SeaLantern/releases/latest)をダウンロードし、サーバーの JAR ファイルをインポートして Java を選択するだけ。あとは「起動」ボタンを押せば完了です。

## 開発

Node.js 20+ および Rust 1.70+ が必要です。

```bash
git clone [https://github.com/SeaLantern-Studio/SeaLantern.git](https://github.com/SeaLantern-Studio/SeaLantern.git)
cd SeaLantern
npm install
npm run tauri dev

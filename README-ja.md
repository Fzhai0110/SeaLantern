# 海晶灯 (Sea Lantern)

Tauri 2 + Rust + Vue 3 をベースにした、軽量な Minecraft サーバー管理ツールです。

## 特徴
* **リアルタイムログ**: コンソールでログをリアルタイムに確認し、コマンドを直接入力可能。
* **server.properties エディタ**: ファイルを手動で編集せず、GUIで設定を変更。
* **ワンクリック管理**: ホワイトリスト、BAN、OP権限を簡単に管理。
* **自動停止**: アプリを閉じる際にサーバーを自動停止し、データの紛失を防止。
* **アップデート確認**: ワンクリックで最新バージョンをダウンロード。

## 技術スタック
* **フロントエンド**: Vue 3 + TypeScript + Vite + Pinia
* **バックエンド**: Rust + Tauri 2
* **スタイル**: 純粋な CSS
* **通信**: Tauri invoke (フロントエンドから Rust 関数を直接呼び出し)

## 開発環境のセットアップ
Node.js 20+ と Rust 1.70+ が必要です。

```bash
git clone [https://github.com/Fzhai0110/SeaLantern](https://github.com/Fzhai0110/SeaLantern)
cd SeaLantern
npm install
npm run tauri dev


Sea Lantern (海晶灯)
Tauri 2 + Rust + Vue 3 ベースの Minecraft サーバー管理ツール
[github-stars] [github-forks] [github-latest]
[gitee-stars] [gitee-forks] [gitee-latest]
[ 简体中文 ] [ English ] [ 日本語 ]
何ができるのか？
 * リアルタイム管理: コントロールパネルでログと負荷をリアルタイムに確認。サーバーへ直接コマンド送信が可能。
 * グラフィカルな設定編集: ディレクトリを探す手間なく、server.properties を GUI で編集。
 * 簡単管理: ホワイトリスト、BAN リスト、OP 権限をスイッチ一つで管理。
 * 安全な終了: アプリを閉じるとサーバーも自動で安全にシャットダウンされるため、セーブデータの破損を防ぎます。
 * ワンクリック更新: アップデートの確認とダウンロードをワンクリックで完結。
クイックスタート
 * Releases からソフトウェアをダウンロードします。
 * サーバーの .jar ファイルをインポートし、Java のバージョンを選択して「Start」をクリック。これだけで完了です。
開発 (Development)
Node.js 20+ および Rust 1.70+ が必要です。
git clone https://github.com/SeaLantern-Studio/SeaLantern.git
cd SeaLantern
npm install
npm run tauri dev

> 注意: Arch などの一部の Linux ディストリビューションでは、npm run tauri dev が直接成功しない場合があります。依存ライブラリが揃っているか確認してください。実行前にパッケージマネージャーで Tauri の依存関係をインストールしておくことをお勧めします。詳細：Tauri | Prerequisites
> 
ビルド:
npm run tauri build

ビルドされたバイナリは src-tauri/target/release/bundle/ に生成されます。
コード品質の確認 (Code Quality Check)
PR（プルリクエスト）を送信する前に、以下のコマンドでコード品質を確認することを推奨します。
フロントエンド:
npm run lint      # チェック
npm run lint:fix  # 自動修正
npm run fmt       # フォーマット

バックエンド:
cargo fmt --all -- --check
cargo clippy --workspace -- -D warnings

技術スタック
 * フロントエンド: Vue 3 + TypeScript + Vite + Pinia
 * バックエンド: Rust + Tauri 2
 * スタイル: CSS
 * 通信: Tauri invoke (フロントエンドから Rust 関数を呼び出し)
 * Electron 不使用、Node バックエンド不使用、Webpack 不使用。高速起動、軽量、低メモリ消費を実現。
計画中の機能 (Planned Features)
以下の機能は既にコードのスケルトン（骨組み）が用意されています。あなたの貢献をお待ちしています：
 * ダウンロードセンター - サーバーコア、プラグイン、Mod のダウンロード
 * バックアップ管理 - セーブデータの増分バックアップと復元
 * イントラネット浸透 - FRP の統合
 * スケジュールタスク - 自動再起動、定期バックアップ、定時コマンド実行
 * リソース管理 - Modrinth や CurseForge からのプラグイン/Mod 検索とインストール
貢献する (Contributing)
貢献は大歓迎です！開始前に [Contributing Guidelines] を一読し、コード規格とワークフローを確認してください。
UI のカスタマイズも大歓迎です！
色は CSS 変数で管理されており、コンポーネントはモジュール化されています。気に入らない部分は自由に変更してください。独自のテーマやスキンの作成、レイアウトの再設計も可能です。
国際化 (i18n)
Sea Lantern は簡体字中国語、繁体字中国語、英語をサポートしています。多言語対応の詳細は src/language/README-en.md を参照してください。
ライセンス
GNU General Public License v3.0
「フレームワークは私たちが作りました。そこに魂を吹き込むのはあなたです。」
💡 接下来你可以：
 * 把这段文字存为 README-ja.md：然后在主 README.md 的顶部加上日语链接。
 * 更新 ja.json：如果你需要我帮你把界面上的按钮（如 "Start", "Import", "Settings"）翻译成地道的日语，请告诉我！

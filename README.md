# Aikome Appendix A Study App

A simple, browser-based flashcard app for studying Appendix A of *Love People — Make Disciples*. Works on PC, tablet, and smartphone. No installation, no account, no internet required after first load.

🇯🇵 [日本語の説明はこちら](#愛込付録a学習アプリ)

---

## Features

- **6 study modes** — Reference → Verse, Verse → Reference, Reference → Topic, Topic → Reference, Mixed, Adaptive, plus a "Weak Verses" mode for tackling tricky ones.
- **Smart suggestions** — When you open the app, it suggests what to study based on your history (weak verses, last session, or starts mixed).
- **Daily goal & streak** — Set a daily target and watch your streak grow.
- **Progress heatmap** — Visualize your mastery of all 34 verses at a glance.
- **Full-text search** across references, verse content, and topics.
- **Topic-grouped browsing** for quick reference.
- **Personal notes** — Add multiple notes per verse, export/import as JSON for backup or device migration.
- **Bilingual** — Switch between Japanese and English with one tap. Settings, study progress, and notes carry over.
- **Adjustable text size** — Useful on smaller screens.
- **Direct link to the JW Watchtower Online Library** for each topic.
- **Single-page web app** — No build step, no dependencies beyond CDN-hosted fonts.

## Requirements

- A modern browser (Chrome, Safari, Firefox, Edge — recent versions).
- That's it. No backend, no database. Your study data lives in your browser's local storage.

## How to Use

### Online (recommended)

Visit the live site:

> 📖 **https://palmspot.github.io/aikome-appendix-a/?key=b7e3a2f8d1c9a0b4e5f6g7h8i9j0k1l2m3n4o5p6**

The `?key=...` portion is required to access the app.

### Offline (download)

1. Click **Code → Download ZIP** above, or clone this repository.
2. Open `index.html` in your browser by double-clicking it.
3. Append `?key=b7e3a2f8d1c9a0b4e5f6g7h8i9j0k1l2m3n4o5p6` to the URL bar after the file path.

> ℹ️ Why the key? It's a soft access barrier so that the URL alone (without the key) won't reveal the app. Anyone reading the source code can find the key — this is by design, not real security.

### Add to Home Screen (iOS)

1. Open the URL in Safari.
2. Tap the share button → **Add to Home Screen**.
3. The app will appear with its own icon and launch fullscreen, like a native app.

## Files

| File | Purpose |
|------|---------|
| `index.html` | All UI, styling, and logic |
| `verses-ja.js` | Japanese verse data (34 entries) |
| `verses-en.js` | English verse data (34 entries) |
| `LICENSE` | MIT License (code only) |

## Data & Storage

All your data — study progress, notes, daily goal, language preference, font size — is stored in your browser's `localStorage`. It never leaves your device.

To back up your notes or move them to another device, use the **Export Notes** button on the Stats tab. The exported `.json` file can be imported on any other device running this app.

## License

The application source code (HTML, CSS, JavaScript) is released under the [MIT License](LICENSE).

The scripture text and topic content are quoted from publications of the Watch Tower Bible and Tract Society of Pennsylvania, including the *New World Translation of the Holy Scriptures* and *Love People — Make Disciples*. Their copyright belongs to the original publishers and is not covered by the MIT License of this repository.

## Acknowledgments

- The English verse texts are short opening phrases from the New World Translation.
- The full text of each verse is available on the official Watchtower Online Library, which the app links to from every verse card.

---

# 愛込付録A学習アプリ

『**愛込（Love People — Make Disciples）**』付録A の暗唱用フラッシュカードアプリです。PC・タブレット・スマートフォンで動作します。インストール不要、アカウント不要、初回読み込み後はオフラインでも動きます。

## 主な機能

- **6つの学習モード** — 書名章節↔聖句、書名章節↔トピック、ミックス、適応学習、苦手攻略
- **スマートな起動時提案** — 苦手のたまり具合や前回の学習に応じて、最適なモードを提案
- **デイリーゴールと連続学習日数** — 毎日の目標を設定し、ストリークを伸ばす
- **習熟度ヒートマップ** — 34節の定着状況を一目で把握
- **全文検索** — 書名章節・聖句本文・トピックを横断検索
- **トピック別一覧** — 主題ごとに節をグループ表示
- **個人メモ** — 各節に複数のメモを保存。エクスポート／インポートで端末間の移行も可能
- **日英切り替え** — ヘッダーのボタンで瞬時に言語切替。学習進捗とメモは共有
- **文字サイズ調整** — 小さい画面でも読みやすく
- **WOL（オンライン・ライブラリー）リンク** — 各カードから該当ページへ
- **単一ページのWebアプリ** — ビルド不要、依存関係はCDNのフォントのみ

## 動作環境

- 最近のブラウザ（Chrome、Safari、Firefox、Edge）
- それだけです。サーバーもデータベースも不要。学習データはブラウザのローカルストレージに保存されます。

## 使い方

### オンラインで使う（推奨）

下のURLにアクセス：

> 📖 **https://palmspot.github.io/aikome-appendix-a/?key=b7e3a2f8d1c9a0b4e5f6g7h8i9j0k1l2m3n4o5p6**

末尾の `?key=...` 部分はアクセスに必須です。

### オフラインで使う（ダウンロード）

1. 上部の **Code → Download ZIP** からダウンロード、もしくは `git clone`
2. `index.html` をダブルクリックでブラウザで開く
3. URL バーのファイルパスの後ろに `?key=b7e3a2f8d1c9a0b4e5f6g7h8i9j0k1l2m3n4o5p6` を追加

> ℹ️ キーが必要な理由：URLだけを知っている人にアプリが露出しないようにする「ゆるい目隠し」です。ソースを見れば誰でも取得できるので、本格的な認証ではありません。

### iOSのホーム画面に追加

1. SafariでURLを開く
2. 共有ボタン → **ホーム画面に追加**
3. ネイティブアプリのようにアイコン＋全画面で起動できます

## ファイル構成

| ファイル | 役割 |
|---|---|
| `index.html` | UI、スタイル、ロジックすべて |
| `verses-ja.js` | 日本語の聖句データ（34節） |
| `verses-en.js` | 英語の聖句データ（34節） |
| `LICENSE` | MITライセンス（コードのみ対象） |

## データと保存先

学習進捗、メモ、デイリーゴール、言語設定、文字サイズ — すべての利用者データはお使いのブラウザの `localStorage` に保存されます。端末から外部に送信されることはありません。

メモをバックアップしたり別の端末へ移行したい場合は、統計タブの **メモをエクスポート** ボタンを使ってください。出力された `.json` ファイルを別の端末でインポートすれば、そのままメモが移ります。

## ライセンス

アプリのソースコード（HTML、CSS、JavaScript）は [MITライセンス](LICENSE) で公開しています。

聖句本文とトピック内容は、ものみの塔聖書冊子協会の出版物（『新世界訳聖書』および『愛を込めて弟子を育てる（Love People — Make Disciples）』）からの引用です。これらの著作権は原典の発行者に帰属し、本リポジトリのMITライセンスの対象には含まれません。

## 謝辞

- 英語版の聖句本文は新世界訳の冒頭フレーズを短く抜粋したものです
- 各節の全文は公式の Watchtower ONLINE Library で読むことができます。アプリ内の各カードからリンクで飛べます

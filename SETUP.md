# GitHub Pages 公開手順 / GitHub Pages Setup Guide

このリポジトリを GitHub Pages で公開する手順のメモです。

## 1. リポジトリ作成

GitHubで新しいリポジトリを作成：

- Repository name: `aikome-appendix-a` （好みで変更可）
- Visibility: **Public**（GitHub Pagesを無料で使うため）
- Initialize with README: **チェックしない**（自前のREADMEを使うため）

## 2. ファイルをアップロード

以下のファイルをリポジトリのルートにアップロード：

- `index.html`
- `verses-ja.js`
- `verses-en.js`
- `LICENSE`
- `README.md`
- `SETUP.md`（このファイル、任意）

ブラウザでファイルをドラッグ＆ドロップでアップロードできます。

## 3. GitHub Pages を有効化

リポジトリの **Settings** → **Pages** へ：

| 項目 | 値 |
|---|---|
| Source | Deploy from a branch |
| Branch | `main` / `/ (root)` |

**Save** を押して数分待つと、`https://YOUR-USERNAME.github.io/aikome-appendix-a/` で公開されます。

## 4. 動作確認

公開URLに `?key=b7e3a2f8d1c9a0b4e5f6g7h8i9j0k1l2m3n4o5p6` を付けてアクセス：

```
https://YOUR-USERNAME.github.io/aikome-appendix-a/?key=b7e3a2f8d1c9a0b4e5f6g7h8i9j0k1l2m3n4o5p6
```

「アクセスが許可されていません」と出ずにアプリが起動すれば成功。

## 5. README のURL を更新

`README.md` 内の `YOUR-USERNAME` を自分のGitHubユーザー名に書き換えて、コミット。

## トラブルシュート

### アプリが真っ白
ブラウザの開発者ツール（F12）を開いてコンソールを確認。`verses-ja.js`、`verses-en.js` が読み込めていない可能性あり。ファイル名や配置を確認。

### ファビコンが古いまま
ブラウザのキャッシュ。ハードリロード（`Ctrl+Shift+R` / `Cmd+Shift+R`）で解決。

### iOS でホーム画面追加してもアイコンが反映されない
一度 Safari の履歴とWebサイトデータをクリアしてから、再度開いて追加。

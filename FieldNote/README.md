# FieldNote セットアップ手順

## ファイル構成

以下のファイルをすべて GitHub リポジトリにアップロードしてください：

- `index.html` — メインHTML（ファイル名は `index.html` のまま）
- `manifest.json` — PWA設定
- `icon-192.png` — アイコン（192x192）
- `icon-512.png` — アイコン（512x512）
- `icon-512-maskable.png` — Android用マスカブルアイコン
- `apple-touch-icon.png` — iOS用アイコン

---

## GitHub Pages デプロイ手順

1. GitHubでリポジトリを作成（例：`fieldnote`）
2. 上記6ファイルを全部アップロード
3. リポジトリの **Settings → Pages** へ
4. **Source: Deploy from a branch / Branch: main / root** を選択
5. **Save** をクリック
6. 数分待つと `https://[ユーザー名].github.io/fieldnote/` で公開

---

## iPhone でホーム画面に追加

1. SafariでGitHub PagesのURLを開く
2. 共有ボタン（□↑）→ **「ホーム画面に追加」**
3. ホーム画面にFieldNoteアイコンが追加される
4. **アイコンから起動するとURLバーが消える**（スタンドアロンモード）

---

## トラブル時

- ホーム画面に追加してもURLが出る → Safariのキャッシュをクリアして再追加
- アイコンが出ない → manifest.json と画像ファイルが同じディレクトリにあるか確認
- 古い画面が出る → 一度ホーム画面から削除して再追加

---

## ファイルの更新

修正したいときは GitHub上で `index.html` を編集すれば反映されます。
ホーム画面のアプリは自動でアップデートされます（リロードが必要な場合あり）。

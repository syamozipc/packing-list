# 持ち物チェックリスト

自分専用のパッキングチェックリスト（旅行・ワーケーション・キャンプ・バックパッカー対応）。
HTML 1ファイルだけの静的サイト。チェック状態は端末の localStorage に保存され、外部送信しない。

## ローカルで開く

```sh
open index.html
```

## GitHub Pages へデプロイ

1. GitHub で空のリポジトリを作る（例: `packing-list`）
2. このディレクトリで:

   ```sh
   git init
   git add .
   git commit -m "init: packing list"
   git branch -M main
   git remote add origin git@github.com:<ユーザー名>/packing-list.git
   git push -u origin main
   ```

3. リポジトリの **Settings → Pages** で
   - Source: `Deploy from a branch`
   - Branch: `main` / `/ (root)` を選んで Save
4. 数十秒後、`https://<ユーザー名>.github.io/packing-list/` で公開される

## カスタマイズ

`index.html` 内の `DEFAULT_DATA` を編集すれば初期リストを変えられる。
カテゴリ・絵文字・項目を自由に追加可能。アプリ上からも項目の追加・削除はできる。

# unimuse-lab プロフィールページ（GitHub Pages用）— たたき台

プロフィールページと改変ガイド一式のたたき台です。このフォルダの中身をそのままリポジトリに置けば公開できます。

## ファイル構成

- `index.html` — プロフィールページ（um.Lab の紹介、BOOTHツール、Kaidoki、ガイドへのリンク）
- `guide/index.html` — 改変ガイドの目次
- `guide/setup.html` — 1. 環境構築：UnityとVRChat SDKの準備（※スクリーンショット枠はダミー。実物の画像に差し替え予定）
- `guide/version-trouble.html` — 2. バージョンが違う・エラーが出たときの切り分け
- `guide/style.css` — ガイド用スタイル

## 置き方（公開手順）

1. リポジトリ `unimuse-lab/unimuse-lab.github.io` のルートに、このフォルダの中身（`index.html` と `guide/` フォルダ）をそのまま置く。
2. リポジトリの Settings → Pages で、公開元が対象ブランチ（通常 `main` のルート）になっていることを確認する。
3. 数分後に `https://unimuse-lab.github.io/` で公開される。

## 差し替えが必要な場所（index.html 内）

- `BOOTH_SHOP_URL`（2か所）: BOOTHショップ um.Lab のURL ← ユーザーから URL をもらう必要あり
- `X_URL`: XアカウントのURL。無ければ Links の X の行ごと削除 ← ユーザー確認が必要
- Kaidoki のリンクは開発リポジトリ（github.com/unimuse-lab/Kaidoki）を指している。サーバー公開時に公開URLへ差し替え。

## 組織名について（決定済み）

- リポジトリは `unimuse-lab/unimuse-lab.github.io` で作成済み。組織名は `unimuse-lab` のまま、公開URLは `https://unimuse-lab.github.io/`。表示名は unimuseLab／um.Lab を使用する。

## 運用メモ

- このページは静的なプロフィール＋ガイド専用。Kaidoki 本体は従来どおりサーバーで動かし、ここからはリンクだけを張る。
- 手順書を増やす場合は、`guide/` に HTML を追加して `guide/index.html` の目次からリンクする。
- 将来 Kaidoki 側に Wiki を移すときは、`guide/` の HTML を持っていけばよい。

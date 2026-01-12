# daenomo.github.io

このリポジトリは個人用の静的サイト（GitHub Pages / Jekyll）です。

## 概要
- サイト: https://daenomo.github.io
- テーマ: `jekyll-theme-cayman`（`_config.yml`で設定）

メモ、ブログ記事（`_posts/`）や単発のページ（*.md）を置いています。

## ローカルでの確認方法
1. 必要であれば Ruby と Bundler をインストールします。
2. （このリポジトリに `Gemfile` があれば）依存をインストール:

```
bundle install
```

3. サイトを起動:

```
bundle exec jekyll serve --livereload
```

（`bundle` を使わない場合は `jekyll serve` でも動きます。）

ブラウザで `http://127.0.0.1:4000` を開くとローカルサイトが確認できます。

## リポジトリ構成（主な箇所）
- `_posts/` : ブログ記事（Jekyll の投稿フォーマット）
- `_config.yml` : サイト設定
- `index.md` : トップページ
- その他の `.md` ファイル: 単独ページ

## 投稿ルール（簡易）
- ファイル名は `YYYY-MM-DD-title.md` の形式で配置します（既存の投稿を参照）。
- フロントマター（YAML）に `title`, `date`, `categories` などを入れてください。

## 連絡・貢献
Issue や PR を歓迎します。緊急の場合は GitHub のプロフィールへ。

## ライセンス
特に明記がない限り、リポジトリ内のコンテンツは作者に帰属します。必要なら LICENSE ファイルを追加してください。

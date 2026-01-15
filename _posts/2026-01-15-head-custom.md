---
layout: default
title: atom追加とhead-custom.html
date: 2025-01-15
---
# head-custom.html ファイルについて
- atomを追加した
  - https://github.com/jekyll/jekyll-feed  
- 追加されたフィード
  - https://daenomo.github.io/feed.xml
- リンクタグを書く必要があった
  - remote_theme なのでテンプレートの直接編集ができない
    - https://github.com/benbalter/jekyll-remote-theme
    - _includes/header.html を追加すれば良いとあるがでてこない
    - 生成されたhtml内のコメントによれば `_includes/head-custom.html` が正しそうだった
    - https://github.com/daenomo/daenomo.github.io/blob/main/_includes/head-custom.html
    - 追加したら出た

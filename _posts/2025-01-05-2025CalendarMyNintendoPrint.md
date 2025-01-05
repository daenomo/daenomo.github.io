---
layout: post
title: 2025 MyNintendoカレンダー印刷
---
# 2025 MyNintendoカレンダー印刷
* 2025 MyNintendoカレンダーをコンビニで写真プリントするために分割する
## 準備
* 以下から日本語のカレンダーをダウンロードする
  * https://my.nintendo.com/rewards/d997adfc1d94bd5a
* ImageMagick をインストールしてパスを通しておく
* カレンダーを保存したディレクトリにて以下を実行する
```bash
i=0;for y in 85 1214 2337; do for x in 36 1252; do ((i++)); convert -crop 1192x974+${x}+${y} -colorspace srgb -density 300 -units PixelsPerInch -scene 1 _2025_Calendar_MyNintendo_Printable_JP_A4.pdf 2025CalendarMyNintendo%d${i}.p
ng;done;done
```

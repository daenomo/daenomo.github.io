---
layout: default
title: 2025 MyNintendoカレンダー印刷
date: 2025-01-05
---
# 2025 MyNintendoカレンダー印刷
* 2025 MyNintendoカレンダーをコンビニで写真プリントするために分割する

## 準備
* 以下から日本語のカレンダーをダウンロードする
  * [2025年 カレンダー（印刷用） \| ギフト \| マイニンテンドー](https://my.nintendo.com/rewards/d997adfc1d94bd5a)
* ImageMagick をインストールしてパスを通しておく
* カレンダーを保存したディレクトリにて以下を実行する

```bash
i=0
for y in 85 1214 2337; do
  for x in 36 1252; do
    ((i++))
    convert -crop 1192x974+${x}+${y} -colorspace srgb -density 300 -units PixelsPerInch -scene 1 _2025_Calendar_MyNintendo_Printable_JP_A4.pdf 2025CalendarMyNintendo%d${i}.png
  done
done
```
2026年版
- [2026年 カレンダー（印刷用） \| ギフト \| マイニンテンドー](https://my.nintendo.com/rewards/7e53d8444a7a61b0)
```
for y in 120 1214 2292; do
  for x in 59 1251; do
    ((i++))
    convert -crop 1170x967+${x}+${y} -colorspace srgb -density 300 -units PixelsPerInch -scene 1 My_Nintendo_YearIn_Review_Calendar_2026_A4_JP.pdf My_Nintendo_YearIn_Review_Calendar_2026_A4_JP%d${i}.png
  done
done
```

## 備考
* ローソンで写真プリントする場合は内接フィットを使うと良い
* ImageMagick v7以降の場合はconvertコマンドがmagickに変更されているため置き換えた方が良いっぽい

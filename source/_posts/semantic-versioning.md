---
title: 五分鐘看懂語意化版本
date: 2018-06-01 15:40:11
tags:
  - 語意化版本
---

## 簡介
語意化版本是一種版本管理規範，但並不是強制規定，所以你當然可以不遵守他提倡的規範，<br>
但被提出來一定是有意義的！

> 以下「應用」指廣義的軟體、函式庫（library）等
開發者在開發應用時，有時候版本的變化會很快速，那麼應該怎麼決定如何 bump 版本？
同時，若使用（include）了其他開發者的應用，要怎麼確保他的更新不會讓你的應用崩盤

## 
版本號以 x.y.z 的型式表示
- x：Major
- y：Minor
- z：Patch

三者會因為不同的原因而有數字的增加，通常從最小單位的 Patch 開始，分別為：
- Patch：解決 Bug
- Minor：增加新功能
- Major：功能無法相法之前的版本

支援運算符
- `>`, `>=`, `<`, `<=`：就跟一般數學的意義相同，不贅述
- `-`：
- `~`： >= 指定版本， < Minor + 1
- `^`： >= 指定版本，< Major + 1
- `x`： >= Minor < Minor + 1
- `*`： 任意 patch
- others: `latest`

[官方網站](https://semver.org/lang/zh-TW/) 是有繁體中文版本的，如果有需要可以前往。
https://docs.npmjs.com/getting-started/semantic-versioning
https://semver.npmjs.com/

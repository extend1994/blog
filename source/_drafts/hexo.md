---
title: Hexo
updated: 2018/05/14
tags: hexo
thumbnail: https://st.nfz.yecdn.com/img/thumbnails/use-hexo-at-any-time-any-place.png
---

## Hexo 介紹

## 文章寫作
Hexo 中預設分為三種，使用使令後會製作一個新檔案到對應資料夾
* post:  `source/_post`
* draft: `source/_draft`，在 web server 中預設是不會顯示的，除非在指令中加上 `--draft`
* page:  `source/`，生成 "目錄"

文章 url： 可以在 \_config.yml [permalink](https://hexo.io/zh-tw/docs/permalinks.html) 欄位設定 test

## 指令與動作
```powershell
# 建立網站
hexo init [<site_name>]

# 寫文章
hexo new [layout:post/draft/page] <title>

# 發表草稿，從 source/_draft -> source/_post
hexo publish [layout] <filename>

# 產生靜態檔案到 "public" 資料夾
hexo generate [-w|--watch]

# 清除快取 (db.json) 與靜態檔案 (public)
hexo clean

# 查看網站狀態
hexo list [page|post|route|tag|category]

# 渲染
hexo render <files> [-o|--output <location>]

# 啟動網頁伺服器瀏覽目前狀態
hexo server [-p|--port] [-s|--static] [-l|--log] [-i <custom_IP>]

# 產生靜態檔案並部署網站
hexo generate -d|--deploy
hexo deploy [-g|--generate]
```
其他選項：safe, debug, silent, draft, config, cwd


### Demo page

https://pseuder.github.io/

### Quick start

```
npm install

hexo server
```

### Troubleshooting

- 'hexo' 不是內部或外部命令、可執行的程式或批次檔。  
  將 hexo 裝到全域 `npm install hexo -g`

### 更新

- 產生靜態檔案(public)  
  `hexo generate`

- 部署至 pages 分支  
  `hexo deploy`

- 若需更新 source code 需推至 master 分支

- 安裝 hexo 自動部署工具(需要時再裝)  
  `npm install hexo-deployer-git`

### 主題

[butterfly](https://butterfly.js.org/posts/21cfbf15/#%E5%AE%89%E8%A3%9D)

### 新增 hexo 專案

`hexo init myblog`

### 新增頁面

`hexo new title`

### 使用自訂 html

```
---
title: 自訂頁面
date: 2023-07-01 15:29:53
tags:
layout: false
---

<!DOCTYPE html>
<html lang="zh-Hant-TW">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
</head>
<body>
  <div class="container">
    <h1>這是標題</h1>
    <p>hi</p>
  </div>
</body>
</html>
```

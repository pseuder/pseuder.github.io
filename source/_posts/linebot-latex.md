---
title: Latex轉換工具
date: 2022-05-15 11:31:59
tags:
  - Python
  - Line bot
  - AWS S3
  - Heroku
---

[Demo video](https://youtu.be/8Zs-yPdhx2s)

<iframe width="560" height="315" src="https://www.youtube.com/embed/8Zs-yPdhx2s" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

# 專案描述

使用者可透過 line 加入好友,  
有 latex 轉換, 極限計算, 微分計算, 積分計算, 共 4 種選項  
點擊對應的功能後傳送對應的數學公式照片即可獲得結果

# 使用技術

- Line bot: 接收使用者輸入與回應
- Python Package
  - Sympy: 計算數學公式
  - Matplotlib: 繪製數學圖形
- Heroku: 雲端託管平台
- AWS S3: 儲存來源與結果照片
- Mathpix API:　圖片辨識 API

# 功能介紹

- Line 介面: 可直接點擊對應區域切換選項
  ![image](linebot.jpg)
- Latex 轉換
  ![image](latex.png)

- 計算結果: 極限、微分、定積分, 不定積分
  ![image](compute.png)
- Heroku
  ![image](heroku.png)
- AWS S3
  ![image](aws.png)

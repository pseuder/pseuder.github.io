---
title: 【實習專案】線上ERP
date: 2022-01-11 01:25:17
tags:
  - Vue
  - Python
  - Django
  - Element UI
  - Sqlite
---

# 專案描述

利用 vue2+django 打造線上 ERP 網站，取代原本的紙本模式

# 使用技術

- 前端: vue2
- css 預處理: scss
- 後端: python
- 應用框架: django
- UI 組件: Element UI
- Router: vue-router
- 資料庫: splite
- 部署平台: heroku

# 功能介紹

- 主要頁面: 列出所有和自己業務有關的產品, 側邊可多選篩選資料
  ![image](main.png)

- 點擊詳細資料可看到該產品的歷史變更紀錄
  ![image](main2.png)

- 提供新增, 修改, 刪除, 延時,下載等功能
  ![image](add.png)
  ![image](edit.png)

- 使用者發出申請後, 審核單位收到信件通知後可至審核頁面審核
  ![image](verify1.png)

- 如有不符規定者可通知補件或否決該筆申請
  ![image](verify2.png)

- 後台首頁提供「審核中資料」「將過期資料」「已申請資料」的概覽
  ![image](backend.png)

- 若使用者為最高級管理群組人員, 則提供「使用者管理」「產品管理」等功能直接操控資料庫
  ![image](backend_user.png)

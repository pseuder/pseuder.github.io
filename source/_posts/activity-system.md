---
title: 活動系統
date: 2023-01-01 14:56:47
top: true
tags:
  - Vue
  - Express
  - Mongoose
  - Tailwindcss
  - AntDesign
  - i18n
  - RWD
---

[Demo](https://pseuder.xyz/activity-system/)
[Github Repository Frontend](https://github.com/pseuder/activity_system)
[Github Repository Backend](https://github.com/pseuder/activity_system_backend)

# 專案描述

此網站為面向公司內部人員的活動報名系統，公司內部人員可以建立與參加自訂活動

# 使用技術

- UI 規劃: [Figma](https://www.figma.com/file/24OpiEY1DoK6SP9hm9h7c0/%E6%B4%BB%E5%8B%95%E5%A0%B1%E5%90%8D%E7%B3%BB%E7%B5%B1?type=design&mode=design&t=B1WdrBut0nmxfA78-1) ![no img](figma.png)
- 前端: Vue3, Pinia, Vite
- 後端: MongoDB + Express.js
- Router: Vue Router
- UI 組件: Ant Design
- CSS 框架: Tailwindcss
- 多國語系: vue-i18n
- 身份驗證: jwt, reCAPTCHA
- 資料驗證: vee-validate, joi
- 第三方登入: Google / Azure / Facebook

- RWD
  <div style="display: flex;">
    <div style="flex: 1; padding: 10px;">
    手機<img src="rwd_login_sm.png" alt="Image 1" >
    </div>
    
    <div style="flex: 3; padding: 10px;">
    平板<img src="rwd_login_md.png" alt="Image 1" >
    </div>

  </div>
  <div >
    電腦<img src="rwd_login_lg.png" alt="Image 1" >
    </div>

# 功能介紹

- 登入畫面
  ![no img](login.png)
- 註冊畫面
  ![no img](signup.png)
- 瀏覽活動, 標籤過濾, 條件排列, 活動狀態, 加入最愛
  ![no img](explore.png)
- 變更排列模式
  ![no img](explore_display.png)
- 活動詳細資訊, 圖片輪播
  ![no img](activity_detail.png)
- 建立活動
  ![no img](create.png)
- 查看跟自己有關的活動(已報名, 已收藏, 已建立)
  ![no img](mine.png)

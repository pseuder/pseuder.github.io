---
title: 日語50音學習網站
date: 2025-04-05 14:56:47
top: true
tags:
  - Vue
  - FastAPI
  - MariaDB
  - Tailwindcss
  - ElementUI
  - i18n
  - RWD
---

線上網站：[https://my-gojuon.vercel.app/](https://my-gojuon.vercel.app/)

# 專案描述

- 提供日語初學者一個隨開隨用的 50 音學習網站
- 針對觸控筆進行最佳優化，方便使用者邊聽邊看邊寫
- RWD 讓使用者隨時快速複習
- 使用 AI 對使用者繪圖進行影像辨識
- 加入 GA 並根據常用國家使用者進行 i18m 多國語系切換

# 使用技術

- 前端: Vue3, Vite, Vercel
- 後端: FastAPI, MariaDB, 自架 GCP VM
- Router: Vue Router
- UI 組件: ElementUI
- CSS 框架: Tailwindcss
- 多國語系: vue-i18n
- 身份驗證: JWT, Google Login
- RWD

# 功能介紹

## 首頁

![no img](home.png)

## 手寫練習

- 跟隨範例與發音熟悉 50 音
- 自動辨識裝置, 支援滑鼠/手指/觸控筆 等方式書寫
  ![no img](writing.png)

## 聽寫練習

- 根據發音書寫對應的文字
- 將畫布上圖案透過 Gemini 進行圖像辨識

  ![no img](listening.png)

## 歌曲推廣

- 提供流行 JPOP 歌曲

  ![no img](songOverview.png)

## 歌曲練習

- 提供歌詞與對照平假名, 並跟隨時間 High Light 當前歌詞
- 中間有分割線可手動調整左右顯示比例
  ![no img](songPractice.png)

## 歌曲設定

- 設定歌曲相關參數(標題, 可見性, 歌詞...)
- 可透過拖放調整歌曲預設順序
  ![no img](backend.png)

## 歌曲編輯

- 將原生歌詞賦予平假名與時間軸標記
  ![no img](songEdit.png)

## GA

![no img](GA.png)

## GSC

![no img](GSC.png)

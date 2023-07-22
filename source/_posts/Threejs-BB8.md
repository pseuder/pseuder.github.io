---
title: Threejs-BB8
date: 2023-07-22 10:38:06
tags:
---

[Demo](https://pseuder.github.io/Threejs-BB8/index.html)
[Github Repository](https://github.com/pseuder/Threejs-BB8)

# 專案描述

透過 Thress.js 建立 3D 物件並使用鍵盤控制移動等功能

- Three.js

  - WebGLRenderer: 基於 webGL 的渲染器
  - Scene: 容納所有 threejs 做出來的 3D 物件
  - PerspectiveCamera: 基於 Perspective 投影法的呈現方式
  - DirectionalLight: 直向光源, 用來呈現陰影, 反光等效果
  - Object3D: 為機器人建立一個 3D 系統, 後續的 Mesh 皆依此為基準
  - Geometry: 3D 物件的形狀
  - TextureLoader: 加載 3D 物件的顏色, 材質等材質
  - Mesh: 將 Geometry 和 Texture 結合
  - OrbitControls: 讓使用者可以用滑鼠自由操控 camara 視角

- 操作&控制

  - 機器人
    - WASD 控制移動方向
    - 上下左右鍵控制頭部轉向
    - 空格跳躍(最多兩次)
    - enter 鍵 發射砲彈
  - 相機視角
    - 滑鼠左鍵按住控制視角
    - 滾輪控制縮放
  - GUI
    - Heading: 唯讀, 顯示當前面向角度
    - Velocity: 唯讀, 顯示當前速度
    - addSpeed: 控制移動時的加速度
    - rotSpeed: 控制轉動時的加速度
    - Stop: 停止移動
    - FollowMe: 將機器人鎖定至 camara 視角中心

- 心得&困難  
   第一次接觸 jacascript, 相比於 c++方便很多, 能做的事情也遠遠超乎我的想像

  在這個作業中, 第一次將以前學過的物理知識融入到程式中, 例如計算當前速度時用到: v ＝ v0 ＋ at, 跳躍時的自由落體用到: y ＝-1/2gt^2

  為了監聽使用者的按鍵, 一開始是直接根據使用者的操作來驅動畫面更新, 但所呈現出來的效果很不順暢, 於是在參考別人的作品後發現 requestAnimationFrame 這個原生函數完美符合我的需求, 使用起來也很方便

# 功能介紹

![image](bb8_1.png)
![image](bb8_2.png)

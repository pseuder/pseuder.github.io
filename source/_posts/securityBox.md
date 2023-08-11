---
title: 樹莓派保險箱
date: 2023-07-22 13:49:40
tags:
  - Python
  - Raspberry Pi
  - IOT
---

[Demo video](https://youtu.be/FsAhyxJDSNM)

<iframe width="560" height="315" src="https://www.youtube.com/embed/FsAhyxJDSNM" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

# 專案描述

以樹莓派為基礎, 打造多功能保險箱

可以透過按壓雲端平台上的虛擬按鈕或手機靠近來解鎖

# 使用技術

Ubidots widget: 雲端平台, 提供虛擬按鈕以供驅動開關
Beacon: 偵測附近的裝置
Line bot: 提供方便的溝通介面
DC GEAR motor: 電動馬達, 可指定角度的轉幅
Buzzer, LED: 發出聲音及燈光
三軸加速度感測器: 可持續偵測 x, y, z 軸的變化
相機: 移動辨識, 拍攝照片
SMTP: 寄送及時通知及照片

# 功能介紹

- 透過設定馬達 0 度與 90 度達到上鎖的效果
  <div style="display: flex;">
    <img src="lock.jpg" alt="Image 1" style="flex: 1; margin: 5px;">
    <img src="unlock.jpg" alt="Image 2" style="flex: 1; margin: 5px;">
  </div>

- 可使用 line bot 或 Ubidots widget 來控制開關
  ![image](linebot.jpg)
  ![image](ubidot.jpg)

- 特定手機靠近時會自動開啟(beacon)
  ![image](beacon.jpg)

- 當上鎖狀態時, 三軸偵測器和照相機同時偵測到變化時，蜂鳴器和 LED 會啟動並將當下照片透過 SMTP 寄送郵件

  ![image](itemmove.jpg)
  ![image](mail.png)

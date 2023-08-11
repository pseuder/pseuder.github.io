---
title: WebGL-照射燈與反射面板
date: 2023-07-16 10:36:01
tags:
  - Javascript
  - WebGL
---

[Demo](https://pseuder.github.io/WebGL-Spotlight-Followers/s1071539_hw2.html)
[Github Repository](https://github.com/pseuder/WebGL-Spotlight-Followers)
[詳細介紹文件](https://github.com/pseuder/WebGL-Spotlight-Followers/blob/master/s1071539_hw2.pdf)

# 專案描述

- 目標

  - 本身有一投射燈，從斜上方照下，永遠照往世界中心點
  - 本身的顏色永遠為暗紅色（不受光線影響）
  - 可調整選轉方向、旋轉半徑、高度等
  - 操作者可透過滑鼠/捲軸調整攝影機的水平跟垂直角度
  - 可視角 60 度、範圍 Z=1~2000
  - 有 15x15 個方形版子，上有貼圖、外有一線框、正面會反射光線，永遠朝向燈光的方向
  - 採用 Phone shading,可調光線顏色、亮度、閃耀度 (shininess)
  - Phone shading：每個向素單獨計算光照
  - 貼圖採用整張貼到物件上，貼圖的顏色會跟光線顏色交互作用

- WebGL

  - Vertex Shader：計算頂點位置、顏色等屬性
  - Fragment Shader：計算每個像素的顏色值
  - Vertex Buffer Object：存儲頂點屬性
  - Element Buffer Object：存儲圖元索引數據
  - GL_TEXTURE_2D：加載並渲染材質
  - gl.bindTexture()：綁定材質到指定的紋理單元上
  - gl.texImage2D()：將圖像上傳到 GPU
  - gl.texParameteri()：設置材質參數，例如放大和縮小
  - gl.enableVertexAttribArray()：開啟頂點屬性數組
  - gl.vertexAttribPointer()：指定頂點屬性數組的格式和數據
  - gl.drawElements()：，Element Buffer Object 繪製
  - gl.clear()：清空 canvas
  - gl.viewport()：設置視口，決定 WebGL 可以在 canvas 繪製的區域大小

- 心得&困難  
   WebGL 屬於較低階的語言, 可以直接和 GPU 溝通, 但在享受最大化效能的同時, 學習門檻也比較高, 除了要知道有哪些函數可以使用, 也要熟悉數學的運算, 例如計算座標位置時用到矩陣乘法, 計算投射燈角度時用到三角函數, 計算打光範圍時用到向量內積等.

  在計算 vertex bufferData 時由於每個平面是由三個點組成, 且根據正反面有順時鐘逆時鐘的差異, 如果搞錯順序會導致無法正確呈現光線效果等問題.

- GUI
  - targetAngle: 投射燈水平角度
  - targetRadius: 投射燈垂直角度
  - targetHeight: 投射燈高度
  - cameraVerticalDeg: 視角垂直角度
  - cameraHorizontalDeg: 視角水平角度
  - lightHue: 光線 Hue 值
  - lightBrightness: 光線亮度
  - Shininess: 光線閃耀程度

# 功能介紹

![image](1.png)
![image](2.png)

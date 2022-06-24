# OpenCV_Tool_Box
## 關於OpenCV 影像創意邁向AI視覺 王者歸來

### 書本重點
核心:
1.之後碰到這概念，或是論文概念，可以再碰到概念的時候，
找對應的code以及執行結果來加深知識理解
2.想辦法輸出一些自己的話，以及focus在deeper processing

1.8-3 影像的加權
2.8-5 影像加密and解密

// 各種thresholod code 加上個人的照片結合
9-1 重要
1.threshold 大於 thresh 取 255 小於取 0
2.threshold 大於 thresh 取 0 小於取 255
9-2
1.Otsu 藉由便利所有閥值，找出最好的方法
2.
3.

9-4 
平面圖分解
太秀了，必須加進去
9-5

11 影像雜訊 Smooth Images

Convolution卷積的定義:
影像與濾波核(Kernel)相乘的動作
大乾貨
11-5 高斯濾波器

11-7 自訂2D Kernel 

12 數學形態學 (Erosion, Dilation)
1.Erosion (利用kernel消除一些與周遭不同的)
EX:將兩顆球一條線連線，變成兩顆球
2.Dilation (利用範圍將自身變成與周遭相同)
EX:將兩顆球中間有空白，變成空白消失
3.開運算 dilate(erode())
4.閉運算 erode(dilate())
5.形態學梯度 Morphological gradient (將膨脹的影像減去腐蝕的影像)
6.禮帽運算top hat (原始影像減去開運算影像)
7.黑帽運算black hat (原始影像減去閉運算影像)

13 影像梯度、邊界
1.影像梯度是指影像強度與顏色方向的變化性

14 影像金字塔

15 輪廓hierachy

17 輪廓的特徵

17-7-2 利用影像實作與醫學找尋身體異常點

18 霍夫變化 Hough Transform (尋找直線、圓形以及橢圓形)

18-1 霍夫變化原理

1.從直角坐標系映射到霍夫空間
2.神奇解釋
霍夫空間上的一個點映射到直角坐標系是一條直線
直角坐標系上的一個點映射到霍夫空間是一條直線
3.極座標(Polar System)與霍夫空間映射的關係

19 均衡化 histogram equalization
1.直方圖均衡化優點:讓彩色或黑白照片 
從暗變明亮
從明亮變暗
往中間靠近
2.直方圖均衡化(Histogram Equalization)有時候會讓照片的細節消失不見，
因此限制自適應直方圖均衡化(ClAHE)，可以有效幫忙解決問題

20 模板匹配 match Template
1.結合計算距離 是一件很厲害的想像

21 傅立葉變換 Fourier Transform (整章都要照做一遍)
1.傅立葉定理:任何的週期性函數都可以由
(1)不同頻率的sin正弦函數(2)不同頻率的cos餘弦函數
所組成
2.實作傅立葉變換
3.

22 分水嶺演算法

23 影像擷取

24 修復蒙娜麗莎的微笑 (太有趣 有時間要嘗試看看)

25 OpenCV與KNN的結合 (非常乾貨的PROJECT) 可以試著跟做一次

27 物件偵測 (很適合當 Project 應用部分 不過數學部分要自己學)

29 LBPH (重要) Local Binary Pattern Histogram (必須要看要學)
1.Eigen Face
2.Fisher Face

30 哈爾分類器
# 通用的爬山演算法架構

* [hillClimbing.js](hillClimbing.js)

## 實作：通用的爬山演算法架構

* [hillClimbingNumber.js](hillClimbingNumber.js)
  * [solutionNumber.js](solutionNumber.js)

```
$ deno run hillClimbingNumber.js
start: energy(0.000)=4.000
0: energy(-0.010)=4.000
1: energy(-0.020)=4.000
5: energy(-0.030)=3.999
7: energy(-0.040)=3.998
8: energy(-0.050)=3.998
9: energy(-0.060)=3.996
11: energy(-0.070)=3.995
...
383: energy(-1.960)=0.158
384: energy(-1.970)=0.119
387: energy(-1.980)=0.080
388: energy(-1.990)=0.040
389: energy(-2.000)=0.000
solution: energy(-2.000)=0.000
```

## 實例 2 ：多變數函數的最佳化

* [hillClimbingArray.js](hillClimbingArray.js)
  * [solutionArray.js](solutionArray.js)

```
$ deno run hillClimbingArray.js
start: energy( 1.000  1.000  1.000 )=1.000
1: energy( 1.000  0.990  1.000 )=0.970
2: energy( 1.000  0.990  1.010 )=0.940
3: energy( 1.000  0.990  1.020 )=0.911
6: energy( 1.000  0.980  1.020 )=0.882
7: energy( 1.000  0.970  1.020 )=0.853
...
786: energy( 2.000  0.500  2.470 )=-2.999
799: energy( 2.000  0.500  2.480 )=-3.000
803: energy( 2.000  0.500  2.490 )=-3.000
804: energy( 2.000  0.500  2.500 )=-3.000
solution: energy( 2.000  0.500  2.500 )=-3.000
```

## 實例 3 -- 排課系統

```
$ deno run hillClimbingScheduling.js

start: score=30.000
 A11:電子 A12:網路 A13:結構 A14:離散 A15:嵌入 A16:演算 A17:網路
 A21:行動 A22:視窗 A23:結構 A24:行動 A25:演算 A26:科學 A27:媒體
 A31:科學 A32:機率 A33:　　 A34:離散 A35:離散 A36:軟工 A37:結構
 A41:系統 A42:機率 A43:智慧 A44:行動 A45:計概 A46:網頁 A47:網站
 A51:結構 A52:軟工 A53:軟工 A54:動畫 A55:結構 A56:計概 A57:工數
 B11:行動 B12:媒體 B13:軟工 B14:電子 B15:網路 B16:線代 B17:演算
 B21:系統 B22:離散 B23:系統 B24:網頁 B25:線代 B26:嵌入 B27:電子
 B31:機率 B32:計概 B33:計概 B34:智慧 B35:機率 B36:系統 B37:計概
 B41:網頁 B42:演算 B43:電子 B44:工數 B45:軟工 B46:電子 B47:網頁
 B51:媒體 B52:機率 B53:線代 B54:結構 B55:行動 B56:機率 B57:網頁
...
solution: score=-3.900
 A11:　　 A12:工數 A13:工數 A14:工數 A15:媒體 A16:媒體 A17:媒體
 A21:　　 A22:線代 A23:線代 A24:線代 A25:嵌入 A26:嵌入 A27:嵌入
 A31:　　 A32:計概 A33:計概 A34:計概 A35:視窗 A36:視窗 A37:視窗
 A41:　　 A42:離散 A43:離散 A44:離散 A45:網站 A46:網站 A47:網站
 A51:　　 A52:軟工 A53:軟工 A54:軟工 A55:演算 A56:演算 A57:演算
 B11:　　 B12:行動 B13:行動 B14:行動 B15:結構 B16:結構 B17:結構
 B21:　　 B22:電子 B23:電子 B24:電子 B25:智慧 B26:智慧 B27:智慧
 B31:　　 B32:科學 B33:科學 B34:科學 B35:系統 B36:系統 B37:系統
 B41:　　 B42:網路 B43:網路 B44:網路 B45:網頁 B46:網頁 B47:網頁
 B51:　　 B52:動畫 B53:動畫 B54:動畫 B55:電子 B56:機率 B57:機率
```
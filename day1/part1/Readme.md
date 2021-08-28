# AI金融科技應用實務 - Day1 課程筆記 - Python底層架構，大家會好奇Python是怎麼讓機器讀懂的嗎?為何Python要多一種翻譯來讓機器讀懂? - Part 1



哈囉，大家好!! 最近小弟決定開始上AI金融科技實體課程培訓，目的是想讓自己更了解AI技術如何在金融產業領域上應用，所以這邊我想紀錄一下，在這個系列課程中我覺得很重要的觀念部分，以及自己多查詢更深入的程式觀念



## 1. Python所具備的特色

把機器執行的細節部分用抽象化的的方法隱藏起來，也就是我們不會看到Python對於電腦的指令執行細節

+ 一行的Python陳述語句可以對應到多行的機器指令

+ 在寫Python的過程無需知道處理器屬於哪種架構

+ 一行指定的陳述語句包括LOAD、STORE和MOVE op-codes

**Python特點**

+ 直譯式語言

+ 開放式原始碼

+　多用途
+　跨平台
+　自動垃圾回收(不需要自己release記憶體，它會自動幫我們執行)
+　動態資料型別
+　適合各種程式撰寫風格
+　用縮排分隔程式區塊



**Python哲學**

在程式中執行

```Python
import this
```

執行結果

```
The Zen of Python, by Tim Peters

Beautiful is better than ugly.
Explicit is better than implicit.
Simple is better than complex.
Complex is better than complicated.
Flat is better than nested.
Sparse is better than dense.
Readability counts.
Special cases aren't special enough to break the rules.
Although practicality beats purity.
Errors should never pass silently.
Unless explicitly silenced.
In the face of ambiguity, refuse the temptation to guess.
There should be one-- and preferably only one --obvious way to do it.
Although that way may not be obvious at first unless you're Dutch.
Now is better than never.
Although never is often better than *right* now.
If the implementation is hard to explain, it's a bad idea.
If the implementation is easy to explain, it may be a good idea.
Namespaces are one honking great idea -- let's do more of those!
```

結果會顯示所有Python中的哲學觀點，也是撰寫Python的原則

**補充**: 其中19條原則被寫了下來，而第20條是要留給Guido van Rossum來寫的，Guido van Rossum是Python程式設計語言最初的設計者和主要的程式架構師



## 2. Python底層架構 - 三階段轉換: Python原始碼 -> 位元組碼 -> 機械碼



**流程圖**

![image1](images\image1.png)

**說明:** 我們所撰寫的Python程式碼在轉換成電腦能夠讀懂的機械碼0跟1中間需要經過兩個階段的轉換，第一階段稱為直譯Interpretation，將我們的程式碼轉換成位元組碼Byte code，接著第二階段透過虛擬機Compilation轉換成最終電腦能夠讀懂的0與1組成的機械碼Machine Code





更多資訊我非常推薦大家閱讀: https://goinglearn.com.tw/programming-languages/151-python-%E7%9A%84%E5%BA%95%E5%B1%A4%E6%9E%B6%E6%A7%8B，我覺得寫得非常清楚完整，作者非常非常厲害









## 3. 為什麼中間要有位元組碼?為什麼不直接轉換成機器碼?

目的是為了讓我們的Python程式碼能夠在不同的作業系統上執行，像是Windows、Mac、Linux

**大家可能會有疑惑，機器碼不是都0、1組成，為什麼不是每個作業系統通用呢?**

這是因為不同作業系統對於0和1組合的解釋都是不同的喔，所以並不通用





## 課程心得

第一堂課的第一部分，老師比較偏重帶大家了解Python程式語言，以便後面實作金融科技技術，所以還沒有進入金融科技的相關知識，但也因為這樣讓我更加了解Python程式語言的觀念，我也因此查了許多關於Python是如何運作的、底層架構、轉換過程等等





## Reference

https://goinglearn.com.tw/programming-languages/151-python-%E7%9A%84%E5%BA%95%E5%B1%A4%E6%9E%B6%E6%A7%8B

https://zh.wikipedia.org/wiki/%E5%90%89%E5%A4%9A%C2%B7%E8%8C%83%E7%BD%97%E8%8B%8F%E5%A7%86




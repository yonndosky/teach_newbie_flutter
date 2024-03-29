# 五月第一週報告
<br>

> # 前言
>> ## 無論學甚麼技術，只要有規則性的就是需要花時間去磨練，沒有捷徑也沒有所謂的有效率的方法學習，所謂的其他人所說的方式只是別人所走過來的方式，不代表自己。
>> <br>
>>
>> ## 當別人問，這一年是如何把Dart語言學好，以及如何面對每個星期的開會時，第一個就是前面說到的就是每天每天花很多時間，再來就是每個星期的開會就好像被追殺一樣，無論如何也要把交代的事情做到好，學多少交多少。

## 進入主題

### 在這就不贅述如何開啟專案，有關於開專案的問題可以參考其他文章。
### 開啟專案後第一個就會看到官方的預設程式，如下圖。

![This is a alt text.](/20220430/onStart1.png)
![This is a alt text.](/20220430/onStart2.png)

## 在看完官方的預設程式時當然假如各位是新手就會有人開始去找runApp是甚麼，stateful和stateless又是甚麼，查資料是一個很好的事情，但是當你查到stateful和stateless是甚麼時，一開始會覺得「既然stateful都用的到，那會甚麼需要stateless」，這個想法很好，那就是代表現階段不用處理這方面的問題，先將問題記起來，等以後真的看越來越多東西之後，或許就會瞭解，亦或是之後突然又想到「好像還沒分清楚stateful和stateless」時再去找資料也來得及，只要開始做了，不管什麼時候做都不嫌晚，所以盡量不要鑽牛角尖在某一行程式碼，這樣會慢慢地因為沒有成就感而失去熱情。
<br>

> # 在看到以上的預設的程式程式時，會發現其實與C++相似。
>> ## 學過龍華科技大学的C++程式設計的人，就可以想起十條規則。
>> ## 除此之外也可以先將註解刪去。

![This is a alt text.](/20220430/rules10.png)

![This is a alt text.](/20220430/clearcode.png)

## 刪除完註解就會獲得如上圖較乾淨的程式碼，而十的規則中也清楚地知道只有第十條，沒有用到，此外也發現了像是MaterialApp,Text,FloatingActionButton...等，()內的引數賦予完之後都會給一個逗號(,)，而這個也就可以成為他的第十條規則。
<br>

## 以上所有的基礎問題釐清後，就可以開始修改程式了，而在這可以先修改Scaffold內的數值，為什麼事先修改Scaffold內，原因就是因為模擬機上也有顯示【You have pushed the button this many times:】的字樣，代表MyHomePage與版面較相關，那上面其他的程式碼就暫且擱置。
## 到這可能有人會說標題也有【Flutter Demo Home Page】字樣為何不是先處理MyApp，原因很簡單，因為MyApp的功能大家會發現，只有賦予顏色，標題以及home使用了MyHomePage作為引數，而且MyHomePage內的關聯度與可改度較高。
![This is a alt text.](/20220430/teach1.png)
<br>

## 第一個做的事情看要改變甚麼，個人在這要直接刪除_incrementCounter()。
![This is a alt text.](/20220430/teach2.png)
## 刪除後，就會發現程式祭出了一個提醒(藍線)與一個錯誤(紅線)，那我們可以先將那兩個錯誤也直接刪除。
<br>

## 刪除後，就會發現程式祭出了更多提醒及錯誤，那就再繼續刪除。
![This is a alt text.](/20220430/teach3.png)
<br>

## 刪除後，就會剩下了一個警告，而現在需要做的事情就是讀懂提醒，將來無論是提醒(藍色)，警告(黃色)，錯誤(紅色)，都需要將他讀懂，因為那行可能是程式需求之一，有可能是語法錯誤，型態錯誤...等;而在這先教一個最快的解決方式，就是點擊警告。
![This is a alt text.](/20220430/teach4.png)
<br>

## 對紅框內訊息點擊一次。
![This is a alt text.](/20220430/teach5.png)
<br>

## 就會發現他將有問題的區域框起，並且多了一個燈泡可點擊，關於燈泡的問題，燈泡就是賦予一些改善想法的工具，那就可以先點擊燈泡看看有哪些參考作法。
![This is a alt text.](/20220430/teach6.png)
<br>

## 通常第一個就會是最佳解，再來參考其發生的提醒，警告，錯誤內容選取適當的調整，在這第一個選項，正好與提醒之內容相似。
![This is a alt text.](/20220430/teach7.png)
<br>

## 點擊後發現問題內的提醒消失，並且沒有其他問題就可以點擊重新整理觀察到模擬機確實產生許多改變，接下來就是可以盡情的查資料與修改。
![This is a alt text.](/20220430/teach8.png)
<br>

# 接下來要介紹的是Google Map的初步寫法。
<br>

## 搜尋後就可能會出現flutter官方或是pub.dev...等參考，在這選擇了pub.dev，除了官方網站，第二優先能夠信任的就是pub.dev，因為他是撰寫flutter時，官方也推薦的網站。
![This is a alt text.](/20220430/google_map1.png)
<br>

## 接下來就可以參考這裡的文獻，去做程式參考，以及修改成為自己需求，在這就不多贅述。
![This is a alt text.](/20220430/google_map2.png)

# 在這根據文獻第一步驟就是先將其引入至pubspec.yaml中，以及更新pubspec.yaml。
![This is a alt text.](/20220430/google_map3.png)
<br>

# 第二步:在main.dart將其import。
![This is a alt text.](/20220430/google_map4.png)
<br>

# 第三步:進入Google Maps Platform網站，並點擊開始使用，並且登入。
![This is a alt text.](/20220430/google_map5.png)
<br>

# 第四步:申請一個新專案。
![This is a alt text.](/20220430/google_map6.png)
<br>

# 第五步:申請一個Api Key。
![This is a alt text.](/20220430/google_map7.png)
<br>

# 第六步:檢查Api Key是否生成，生成的話就點擊編輯。
![This is a alt text.](/20220430/google_map8.png)
<br>

# 第七步:編輯Api Key。
![This is a alt text.](/20220430/google_map9.png)
<br>

# 第八步:複製Api key。
![This is a alt text.](/20220430/google_map10.png)
<br>

# 第九步:回到文獻參考，並且照文獻描述位置加入特定程式碼，並將剛剛複製的api key放至紅色實心區域。
![This is a alt text.](/20220430/google_map11.png)
<br>

# 第十步:複製程式碼至main.dart並執行。
![This is a alt text.](/20220430/google_map12.png)
<br>

# 第十一步:瞭解程式碼並且互動。
![This is a alt text.](/20220430/google_map13.png)
<br>

# 最後的最後就是開始修改程式查看更多資料，將要求做出來。
# 這裡假設是輸入經度或緯度後能有立即改變，那將程式碼稍作修改，充分理解後，再將其實現。
## 程式碼大致介紹。
![This is a alt text.](/20220430/change1.png)
<br>

## 介紹TextField的工作，在這只介紹textfieldX，因為textfieldY是一樣的。
![This is a alt text.](/20220430/change2.png)
<br>

## 介紹showMap的工作。
![This is a alt text.](/20220430/change3.png)
<br>

## 介紹_goToEveryWhere。
## 在這先講解controllerMap.future，將游標移至時，根據內容為等待該控制器在complete或completeError呼叫，而前面就已經讓控制器的complete完成了，所以這一行確認完畢就會執行下一行。
![This is a alt text.](/20220430/change4.png)
<br>

![This is a alt text.](/20220430/change5.png)

## 初始畫面
![This is a alt text.](/20220430/show0.png)
<br>

## 展示一
![This is a alt text.](/20220430/show1.png)
<br>

## 展示二
![This is a alt text.](/20220430/show2.png)
<br>

## 展示三
![This is a alt text.](/20220430/show3.png)
<br>

# 以上感謝各位的聆聽!

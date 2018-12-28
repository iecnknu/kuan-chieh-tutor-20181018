# Bootstrap 4

##### 🗒️什麼是Bootstrap?

在上一章我們學到CSS可以外置、直接呼叫檔案來套用，比起設定&lt;style&gt;標籤快上不少；但就算這樣，CSS內的各式屬性值仍然需要人為調整、一步一步動手刻，對於不擅美術設計的人來說，相當費時耗神。

所以聰明的工程師們想到了一套方法，讓我們直接套用專業美術人員設計的CSS類別，其內容幾乎涵蓋了所有會圖像化顯示的標籤，而這就是Bootstrap 4。\(4表示第四代\)

![](https://drive.google.com/uc?export=download&id=1j6XsdjwL6phRwugcj9hr3tNjhYq88MLd)

---

##### 🗒️試試Bootstrap 4！

我們的目標是將自己打造的Google首頁，透過Bootstrap美化、看起來更像真的首頁。  
不管是輸入框、按鈕、字體、排版等，似乎都比原本的好看了不少！

![](https://drive.google.com/uc?export=download&id=1wj5OoYdKuiSPScepw9x8rl61JLbuuy0w)

1. **匯入CSS**  
   先進到[Bootstrap首頁](http://bootstrap.hexschool.com/docs/4.0/getting-started/introduction/)，找到CSS這個大標題，依照提示將該&lt;link&gt;標籤加入&lt;head&gt;標籤之中。  
   ![](https://drive.google.com/uc?export=download&id=1AXZ4zh4WEU4ycw9eFad6lFxAZ2E4sXf8)

   ```php
   <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/css/bootstrap.min.css" integrity="sha384-Gn5384xqQ1aoWXA+058RXPxPg6fy4IWvTNh0E263XmFcJlSAwiGgFAW/dAiS6JXm" crossorigin="anonymous">
   ```

   這會使用CDN，讓你的網站被瀏覽時，快速的將Bootstrap的CSS檔案下載到瀏覽者的電腦中。  
   這樣一來可以減輕小型開發者伺服器的負擔。

2. [基本排版元素](http://bootstrap.hexschool.com/docs/4.0/layout/overview/)  
   container是類別是Bootstrap最基本的排版元素，它可以控制網站在整個螢幕上面顯示的比例。  
   在一些視覺設計的研究指出，透過留白，可以引導使用者的眼神留在最重要的區域。而左右留白的比例分別是15%左右。  
   為了讓整個網站都能被更好的閱覽，我們將&lt;body&gt;標籤套用container類別。

   ```php
   <body class="container">
   ```

3. **form元件**  
   1️⃣請在Bootstrap網站左側的導覽列，選擇元件。  
   2️⃣在展開的各元件標題中找到【[表單 \(Forms\)](http://bootstrap.hexschool.com/docs/4.0/components/forms/)】。  
   3️⃣找到範例中要套用在&lt;form&gt;標籤上的類別：form-group。  
   4️⃣輸入框的&lt;input&gt;標籤，則使用類別：form-control，進行樣式化。  
   5️⃣以上兩個步驟可以對這些標籤樣式化，包括一般外觀、focus 狀態、尺寸等等的樣式。  
   輸入框是不是出現原角了呢？

4. **麥克風圖示**  
   1️⃣在展開的各元件標題中找到【[Input 群組 \(Input group\)](http://bootstrap.hexschool.com/docs/4.0/components/input-group/)】。  
   2️⃣它可以輕鬆擴展表單控制元件加入文字內容、按鈕、按鈕群組、其他周圍的文字、自訂選單、自訂檔案欄位等。  
        麥克風圖示就是在輸入文字框後加上一張小圖，一樣使用&lt;img&gt;標籤新增。

   ```php
        <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/e/e8/Google_mic.svg/2000px-Google_mic.svg.png" width="20" height="28">
   ```

   3️⃣我們要將輸入框和小圖組合成一個群組：新增`<div class="input-group">`將想要組合的元件包起來。  
   4️⃣將要抽入在後面的元件，新增`<div class="input-group-append">`標籤包起來。  
   5️⃣將要抽入在後面的元件內容，新增`<span class="input-group-text">`標籤包起來。

5. **按鈕元件**  
   1️⃣在展開的各元件標題中找到【[按鈕 \(Buttons\)](http://bootstrap.hexschool.com/docs/4.0/components/buttons/)】。  
   2️⃣在&lt;form&gt;裡面的`<input type="submit" value="Google 搜尋" >`，也是一種按鈕，我們可以直接套用按鈕元件的類別。  
   3️⃣將其套用外觀最相近的類別`btn btn-light`

6. **大功告成！**  
   接下來可以設定[更細節的邊框](https://www.w3schools.com/cssref/pr_border-left.asp)、按鈕顏色、container的寬度等，讓網頁更像Google喔！  
   ![](https://drive.google.com/uc?export=download&id=1d0SQWEp-GKWiZoUF1UiHwA-OVH21EJxa)

---

##### 




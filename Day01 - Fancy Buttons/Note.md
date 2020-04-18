## **Day1 Note**

---

### `本日主要內容 -- 建立五種不同的按鈕(各含兩種型式)`



#### 1. Facebook style - dark & light

首先是一般按鈕，分別是深色版及淺色版，並各自於`:hover`及`:active`設計滑鼠滑過及按住時，按鈕呈現較深色的狀態

#### 2. 3D Buttons - Rectangle & Circle

製作兩個3D按鈕(方形和圓形)，並設計呈現出滑鼠滑過及按下時的狀態

1. 方形: 運用`::before`及`::after`設計出兩個小三角形去填補下方陰影處的空隙(左下右下)，讓按鈕整體呈現出3D樣式，因為進入`:active`狀態時按鈕呈現按下樣式，故`::before`及`::after`也需加入`:active`狀態來進行調整

2. 圓形: 利用`box-shadow`堆疊出圓形的陰影來呈現出3D樣式，並運用`radial-gradient`來設計出兩個顏色放射漸變的圓形背景

#### 3. Gradient Bordered Buttons

設計兩個不同漸變方式的按鈕，兩者皆使用`linear-gradient`來設計按鈕呈現漸變色背景，是運用`:hover`來操作按鈕狀態，其中第二個按鈕因設計漸變成透明色，`:hover`中加入取消右邊的boder樣式


#### 4. Animated Buttons

設計兩個不同方式讓按鈕呈現動畫效果

1. 按鈕加入背景圖片後，運用`animation`讓按鈕呈現背景滾動的動畫效果
2. 利用`::after`在按鈕內文子後方加入">>"，將">>"先預設為為透明(`opacity: 0`)，並於`:hover::after`中改為不透明(`opacity: 1`)顯示在畫面中，以達到動畫效果

#### 5. Toggle Switch UI Buttons

將checkbox設計成開關按鈕，利用`::before`設計按鈕一開始狀態，並運用`:checked`來設計按鈕被選中時的狀態(`:checked + button` 及 `:checked + ::before`)

---

### **`補充 --`**

* text-shadow:  offset-x | offset-y | blur-radius | color
  * 為文字添加陰影，可添加多個陰影，陰影值用逗號隔開

* box-shadow:  inset | offset-x | offset-y | blur-radius | spread-radius | color
  * inset的存在將陰影改為幀內陰影，在邊框內部繪製插入陰影
  * blur-radius: 值越大、模糊越大、陰影越大(不可使用負值)
  * spread-radius: 正值將陰影擴大變大，負值將陰影縮小
* ::before ::after
  * 兩個冒號開頭(::)為偽元素，一個冒號開頭(:)為偽類
  * ::before 在原本的元素之前加入內容
  * ::after 在原本的元素之後加入內容
  * 偽元素必備content屬性意旨插入的內容，可是文字、圖片、網址等，如未填此屬性，偽元素將不會發生作用

* outline
  * 元素的外圍邊框(輪廓線)

* position:  static | relative | absolute | fixed | sticky
  * static 默認，即當前布局狀態
  * relative 表現和默認一樣，但可增加屬性來相對調整位置(top、right、left、bottom)，而不管這些相對定位過的元素一位置或增加多少空間都不會影響原本其他元素所在位置
  * absolute 固定定位在元素所處的上層容器的相對位置(top、right、left、bottom)，如無上層容器則訂於該網頁的所有內容(body)
  * fixed 固定定位元素會瀏覽器視窗來定位(top、right、left、bottom)，意味即使頁面捲動，他還是會在固定的相通位置
  * sticky 滾動黏滯定位(常用於navbar)

* radial-gradient:  position | shape | extent-keyword 
  * 創建一從原點輻射開並用兩個或多個顏色間漸變組成的圖片，屬於image屬性
  * position 設定漸變位置，默認為center
  * shape 設定漸變的形狀，值可以是circle或ellipse，默認為ellipse
  * extent-keyword 設定結束形狀必須多大的關鍵字(closest-side、closest-corner、farthest-side、farthest-corner)

* animation & @keyframes
  * animation 可以設定元素動畫效果，參數 name | duration | timing-function | delay | direaction | fill-mode | play-state ，按照需求選用，但必須要有name
  * 設定好animation後可用@keyframese關鍵影格調用動畫開始(from)到結束(to)位置 

* vertical-align: abseline | top | middle | bottom | super | sub | text-top
  * 指定行內元素或表格單元格的垂直對齊方式

* :checked
  * 表示任何處於選中狀態的元件(radio、checkbox、option)
  * :checked 後面使用加號意思是選到後方，只能選到後面的第一的元件


## **Day6 Note**

---

### `本日主要內容 -- 讓列印機可以漂亮輸出的樣式`

#### 1. 建立出專屬列印使用的版面

`@media`除了可以來製作響應式網頁外，還可以使用於創建專屬列印產生的畫面(於預覽列印中顯示)，運用`@media print`來操作調整版面，不需要顯示的物件可採用`display: none;`遮蔽，文字、特效等，則是網頁情形進行調配，如`a`標籤中網址顯示出來，可以利用`::after`於`content`放入`attr(href)`

---

### **`補充 --`**

- @media
  - 常用類型: all、print、screen、speech
  - 常用特徵:
    1. 視窗或頁面尺寸(width、height、aspect-ratio、orientation)
    2. 顯示品質(resolution、scan、update、overflow-block、overflow-inline、grid)
    3. 顏色(color、color-index、monochrome、color-gamut)
    4. 互動(pointer、hover)
  - 使用方式: or(,)、and、not、only
  - [MDN--media](https://developer.mozilla.org/en-US/docs/Web/CSS/@media)

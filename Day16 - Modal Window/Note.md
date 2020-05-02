## **Day16 Note**

---

### `本日主要內容 --`

#### 1. 運用 CSS 實現彈出及關閉互動視窗

使用`position:fixed`將互動視窗完成定位並將互動視窗設定透明(`opacity: 0`)，只有在`checkbox`處於`:checked`狀態時，`checkbox`以下的互動視窗相關內容(`.overlay .modal`)顯示於頁面(`opacity: 1`)

---

### **`補充 --`**

- pointer-events

  - 針對滑鼠事件的屬性，預設值為 auto，如設定值為 none，則可以穿越該元素，點擊下方的元素，除了 auto 及 none，其他設定值基本上是適用於 SVG 內容
  - [MDN--pointer-events](https://developer.mozilla.org/en-US/docs/Web/CSS/pointer-events)

- Selector

  - A + B: 相鄰選擇器，可選擇有相同父元素，緊鄰著 A 元素後的第一個同層 B 元素
  - A ~ B: 間接選擇器，可選擇有相同父元素，且 A 元素以下的所有同層 B 元素
  - [MDN--Selector](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Selectors)

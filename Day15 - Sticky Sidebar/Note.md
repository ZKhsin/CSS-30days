## **Day15 Note**

---

### `本日主要內容 --`

#### 1. 建立固定的側邊欄

運用`float`及`position: fixed`實現側邊欄在固定位置，並滾動畫面時一併隨著頁面移動，特別注意因為使用`float`，為了防止頁尾跑版，故需運用`::after`創造一個塊狀區域設定`clear: both`

---

### **`補充 --`**

- clear
  - 當使用 float 元素時，由於區塊是浮動的，若接下來的區塊為使用 float 時便會產生跑版的現象，此時須適當使用 clear 來解決問題
  - 使用值: left、right、both、none、inherit(IE 不支援)

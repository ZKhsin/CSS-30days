## **Day3 Note**

---

### `本日主要內容 -- 運用clip-path剪裁出不同形狀的圖片`



#### 1. 圓形

運用`clip-path`中的`circle`來繪製剪裁出圓形形狀

#### 2. 對話框、X、箭頭

因這三種形狀都須利用點座標的方式來剪裁形狀，故運用`clip-path`中的`polygon`來繪製剪裁出形狀



---

### **`補充 --`**

* clip-path clip-source | [ basic-shape || geometry-box ] | none
 * clip-paht可以創建一個只有元素的部分區域顯示的剪裁效果，剪裁區域內顯示，區域外則隱藏
 * [MDN--clip-path](https://developer.mozilla.org/en-US/docs/Web/CSS/clip-path)
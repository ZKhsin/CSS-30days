## **Day4 Note**

---

### `本日主要內容 -- 建立帶有特效的表單`

#### 1.設計表單外背景及表單內樣式

先運用`linear-gradient`來設計表單外背景，再進入逐步設計表單內容，這裡有使用到`:not`來設計除了 submit 以外的元素，並額外針對 submit 背景帶入`linear-gradient`來設計出斜紋樣式及運用`:hover`設計出移動到 submit 上產生斜紋變大的效果

#### 2. 表單設計往下呈現展開兩層的特效

利用`::beofre`跟`::after`建立出兩塊版面在表單後方，於`:hover`時運用`transform`中的`scale`及`translate`來顯示出來兩塊版面，另讓`::after`使用`transition-delay`延遲出現來達到兩塊版面依序出現的效果

---

### **`補充 --`**

- linear-gradient( [angle | to side-or-corner ,]? color-stop-list )
  - angle & to side-or-corner 用於定義漸變線角度或起始點位置，color-stop-list 由多個 color 值所組成(可以使百分比搭配或沿著漸變軸的長度)
  - angle: 使用 deg 來指定漸變方向或角度；to side-or-corner: 使用 to 加上兩個關鍵詞(水平位置、垂直位置)，關鍵詞可為 top、left、right、bottom

---

### **`新增 --`**

新增一表單，並增加響應設計

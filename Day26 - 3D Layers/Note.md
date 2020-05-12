## **Day26 Note**

---

### `本日主要內容 --`

#### 1. 製作 3D 圖層效果

運用將元素設置位於 3D 空間(`transform-style: preserve-3d`)，並使用`transform`製作出分層圖層效果

---

### **`補充 --`**

- transform-style

  - flat: 設置元素的子元素位於該元素的平面中
  - preserve-3d: 設置元素的子元素位於 3D 空間中

- perspective

  - 設置 transform 3D 的透視，設定的值可以想像成物件距離螢幕的距離，值越大代表越遠，越小代表越近

- Z
  - rotateZ: 控制元素繞著 Z 軸旋轉
  - translateZ: 3D 空間中 Z 軸，控制元素移近移遠，數字越大元素越近，數字越小元素越遠

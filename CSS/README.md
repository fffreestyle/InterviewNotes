#### 1. CSS `left` and `translate` 有何不同

left 為從畫面最左邊開始計算

translate 為根據他本身的 width 去計算

#### 2. box model

每個 DOM 元素都可以被視為一個 box 從外而內為 margin、border、padding 和 content

#### 3. stack context

指 CSS 中 z-index 的元素堆疊模式類似圖層堆疊

#### 4. position 

static 為預設，瀏覽器自動排列

relative 可以設定 top, left, right, bottom 等屬性根據其他元素位置做定位不會影響到其他元素的空間

fixed 會根據瀏覽器畫面做定位

absolute 根據上層容器做定位，但 static 為例外
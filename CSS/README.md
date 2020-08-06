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

absolute 根據上層容器做定位，但如果上層容器是 static 便會忽略繼續往上尋找

#### 5. restting 和 normalizing

restting 透過消除不同瀏覽器的 default 樣式，來達到在不同瀏覽器都有一樣的畫面

normalize 留下有用的 default 樣式並盡量保持瀏覽器的顯示一致性

#### 6. Block Formatting Context

是指這個區塊的布局方式是透過 block 和 inline 的規則呈現
#### 請解釋什麼是 controlled component 跟 uncontrolled component
主要是在表單輸入相關的元件。
以原生 input element 為例，輸入欄中的顯示資料是由 DOM 本身的 state 去管控，因此為 uncontrolled(不由 React 管理)。
而 controlled 則是指在 input 中輸入訊息是(觸發 onChange)，會先去 update react 的 state，在由這個 state 決定該元件要顯示的值，因為是由 react 控制，所以稱作為 controlled component。

#### 請解釋 key 的作用？state 跟 props 差在哪裡
key 是用來讓 react 可以辨別是否為不同的 element 以進行新增修改與刪除。
state 是由元件去維護並且可以根據使用者互動等事件去更新。
props 則是由上層元件傳下來，因此並無法更動，只能拿來使用。

#### React 是怎麼運作的

React 使用 virtual-DOM 來透過 JS 控制畫面上顯示的 DOM 元素，並使用他尋找差異的演算法去更新畫面

#### Virtual-DOM 怎麼運作

因為 DOM 本身就是樹狀結構，因此可以透過 JS 來創建出類似的物件結構，先對 JS 本身的結構去做運算，之後再實際 render 到畫面上，減少運算中一直導致畫面重新計算的浪費

#### JSX

一種 JS 的語法擴充，而因為 React 是直接透過 JS 在控制畫面元件，因此透過 JSX 讓工程師在 coding 的時候可以比較直觀的使用類似 HTML 的結構做控制

#### HOC(higher order component)

算是一種 pattern 透過將 react 的 component 當參數傳入經過處理之後再 return 一個新 component ，透過這種方式可以將程式中重複使用到的地方抽出，來讓不同的 component 共用。如 redux 的 connect 讓需要存取 state 的 component 都可以連結

#### refs

可以直接去存取 DOM 元素本身

#### hook

讓 functional component 可以擁有本地的 state，而且提供一個比較直觀的 coding 方式

#### useState

讓 functional component 擁有本地的 state

#### useEffect

用來執行一些有 side effects 的時候使用
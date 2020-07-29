#### 請解釋什麼是 controlled component 跟 uncontrolled component
主要是在表單輸入相關的元件。
以原生 input element 為例，輸入欄中的顯示資料是由 DOM 本身的 state 去管控，因此為 uncontrolled(不由 React 管理)。
而 controlled 則是指在 input 中輸入訊息是(觸發 onChange)，會先去 update react 的 state，在由這個 state 決定該元件要顯示的值，因為是由 react 控制，所以稱作為 controlled component。

#### 請解釋 key 的作用？state 跟 props 差在哪裡
key 是用來讓 react 可以辨別是否為不同的 element 以進行新增修改與刪除。
state 是由元件去維護並且可以根據使用者互動等事件去更新。
props 則是由上層元件傳下來，因此並無法更動，只能拿來使用。

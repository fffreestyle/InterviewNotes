
#### 1. .bind 、 .call 和 .apply有何不同？
* fun.bind(thisArg[, arg1[, arg2[, ...]]])

    thisArg 為想傳入 function 當作 function 中 this 的值
    
    後面的 arg1 ... 將會是執行此 function 直接被帶入的參數

    fun.bind() 之後不會執行 fun

* fun.call(thisArg[, arg1[, arg2[, ...]]])

    thisArg 為想傳入 function 當作 function 中 this 的值
    
    後面的 arg1 ... 將會是執行此 function 直接被帶入的參數

    fun.call() 之後會立即執行 fun

* fun.apply(thisArg, [argsArray])

    thisArg 為想傳入 function 當作 function 中 this 的值

    [argsArray] 將會是執行此 function 直接被帶入的參數

    fun.apply() 之後會立即執行 fun


#### 2. == 和 === 有什麼不同？

在 JS 中 == 會根據兩邊的值去自動轉換型別再做比較

=== 為不做型別轉換直接使用目前的型別做比較

#### 3. Immutable 是什麼？

指操作變數的時候不變動原本的值，而是將結果用新的變數回傳

#### 4. 同步（synchronous）與非同步（asynchronous）函式之間的差異

同步函式為此函式的運算處理完之前，此 thread 會持續處理此函式直到結束才能做其他事情

非同步函式為執行當下不需要等待函式回傳，而是透過 callback 在函式有結果時處理

#### 5. Event Loop

function 呼叫時會被放入 call stack 中執行完就會被 pop 出去

而非同步函式一開始會先丟入 call stack 中讓瀏覽器執行，便會從 call stack 中 pop

非同步函式有結果之後會將該函式的 callback function 放入 callback queue 中，等待 call stack 為空便將 callback function 放入 call stack 執行

 event loop 就是不斷偵測 call stack 是否為空，為空便將 callback queue 中的函式放入 call stack 執行

#### 6. [看 Code 題目](https://github.com/fffreestyle/web-interview-questions/blob/master/JavaScript/%E7%9C%8B%20Code%20%E9%A1%8C%E7%9B%AE)

#### 7. 請解釋什麼是 side effect
執行一個 function 的時候會影響到外部 scope 的值。
#### 8. CORS 是什麼
是一種 HTTP header，必須包含 CORS 才可以進行跨領域請求
#### 9. 請解釋 dom 的事件傳遞

User 觸發事件後，事件由最外層 dom 向下傳遞(CAPTURING_PHASE)直到 User 觸發的目標(AT_TARGET)，再將此目標資訊放入事件傳遞中向上回傳(BUBBLING_PHASE)

addEventListener 有第三個參數，沒有傳預設為 false 代表這個 listener 為冒泡階段觸發

e.stopPropagation 中斷向下傳遞使用

e.preventDefault 為取消瀏覽器的預設行為(如點擊超連結不開新分頁或跳轉)

#### 10. 請解釋 closure 是什麼

假設有一個外層 function 裡面有一個變數和一個內層 functuon 裡面有使用到外層的變數

然後我們如果直接在別的地方呼叫內層 function 仍然可以正常存取原本屬於外層的變數

這個變數被存在內層 function 理的現象就是 closure

你孫子跟你說他有 10 元 然後隔天他就忘了 於是她來問你說 他有多少錢 你就能跟她說她有10元 這就是closure

#### 11. 原型鍊 *(待討論)

盡頭為 Object.prototype

A.__proto__ 指向 A 的 parent

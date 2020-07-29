
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


#### 2. [== 和 === 有什麼不同？](https://github.com/fffreestyle/web-interview-questions/blob/master/JavaScript/%3D%3D%20%E5%92%8C%20%3D%3D%3D%20%E6%9C%89%E4%BB%80%E9%BA%BC%E4%B8%8D%E5%90%8C%EF%BC%9F.md)
#### 3. [Immutable 是什麼？](https://github.com/fffreestyle/web-interview-questions/blob/master/JavaScript/Immutable%20%E6%98%AF%E4%BB%80%E9%BA%BC%EF%BC%9F.md)
#### 4. [同步（synchronous）與非同步（asynchronous）函式之間的差異](https://github.com/fffreestyle/web-interview-questions/blob/master/JavaScript/%E5%90%8C%E6%AD%A5%EF%BC%88synchronous%EF%BC%89%E8%88%87%E9%9D%9E%E5%90%8C%E6%AD%A5%EF%BC%88asynchronous%EF%BC%89%E5%87%BD%E5%BC%8F%E4%B9%8B%E9%96%93%E7%9A%84%E5%B7%AE%E7%95%B0.md#%E5%90%8C%E6%AD%A5synchronous%E8%88%87%E9%9D%9E%E5%90%8C%E6%AD%A5asynchronous%E5%87%BD%E5%BC%8F%E4%B9%8B%E9%96%93%E7%9A%84%E5%B7%AE%E7%95%B0)
#### 5. [看 Code 題目](https://github.com/fffreestyle/web-interview-questions/blob/master/JavaScript/%E7%9C%8B%20Code%20%E9%A1%8C%E7%9B%AE)
#### 6. 請解釋什麼是 side effect
執行一個 function 的時候會影響到外部 scope 的值。
#### 7. CORS 是什麼
是一種 HTTP header，必須包含 CORS 才可以進行跨領域請求
#### 9. 請解釋 dom 的事件傳遞

#### 10. 請解釋 closure 是什麼

假設有一個外層 function 裡面有一個變數和一個內層 functuon 裡面有使用到外層的變數

然後我們如果直接在別的地方呼叫內層 function 仍然可以正常存取原本屬於外層的變數

這個變數被存在內層 function 理的現象就是 closure

你孫子跟你說他有 10 元 然後隔天他就忘了 於是她來問你說 他有多少錢 你就能跟她說她有10元 這就是closure

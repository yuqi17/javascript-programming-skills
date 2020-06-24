参考：[https://www.cnblogs.com/wjw1014/p/10507060.html](https://www.cnblogs.com/wjw1014/p/10507060.html)

首先，rxjs 中的 Observable 是跟 Promise 类似的。但是前者要强大很多，可以专门用来处理各种数据，可取消，还可以对数据进行加工。
其次它的概念不同：Observable 被声明为 可观察对象：可以是字面量，消息和事件。新的版本有专门的operator 来编写，比如of,fromEvent
让代码更加的独立。

Observable 相当于是一个数据仓库：其中的一个回调函数 被称为：订阅者（subscriber）函数，这个对象有一个subscrible 函数是一个消息处理器，其中
有一个函数是observer 被称为 观察者。对于数据来说，产生数据的是生产者比如事件源，使用最终数据的是消费者比如界面模板

rxj中还有一个概念叫主体 Subject 跟 Observable 的功能不太一样，它是一次性的。

subscription = observable.subscribe 这个就是订阅，它是可以随时取消的，还有一个专门控制订阅的叫调度器。

基本概念如下：
(https://cn.rx.js.org/manual/overview.html)[https://cn.rx.js.org/manual/overview.html]

这个东西它属于一种新的编程范式：响应式编程：一切都是流，跟函数式编程，面向对象编程和面向过程编程又不一样。其实这些范式和模式都不过是思维的一种
提炼，没有谁对谁错，只有用对了场景，才能发挥最大的效益。

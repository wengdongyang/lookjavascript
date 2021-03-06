# Hoisting（变量提升）

变量提升：在指定作用域里，从代码顺序上看是变量先使用后声明，但运行时变量的“可访问性”提升到当前作用域的顶部，其值为`undefined`，没有“可用性”。

首先纠正下，文章标题里的“变量提升”名词是随大流叫法，“变量提升”改为“标识符提升”更准确。因为变量一般指使用`var`声明的标识符，JS里使用function声明的标识符也存在提升（Hoisting）。

JS存在变量提升，这个的设计其实是低劣的，或者是语言实现时的一个副作用。它允许变量不声明就可以访问，或声明在后使用在前。新手对于此则很迷惑，甚至许多使用JS多年老手也比较迷惑。但在 ES6 加入 let/const 后，变量Hoisting 就不存在了。

这个"设计"显然是有问题的。

## Reference

- [JavaScript中变量提升是语言设计缺陷](https://www.cnblogs.com/snandy/p/4552078.html)

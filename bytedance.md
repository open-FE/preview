简答题

1.解释一下基于prototype的继承是如何实现的

2.解释一下attribute和property的区别

3.标准模式(Standard Mode) 与混杂模式(Quirks Mode)有什么区别？ 他们的意义编程题

编程题

1.给一颗二叉树，和一个值，检查二叉树中的是否存在一条路径，这条路径上所有节点的值加起来等于给定的那个初始值。例如下面的二叉树，如果初始值是22，那么存在一条路径 5 -> 4-> 11 -> 2。
```
          5
         / \
        4   8
       /   /  \
      11  13   4
     /  \       \
    7    2       1
请实现如下这个函数
function hasPathSum(){
  // 请输入答案
}
```

2.请实现如下的函数，可以批量请求数据，所有的URL地址在urls参数中，同时可以通过 max 参数控制请求的并发度，当所有请求结束之后，需要执行callback回调函数。发请求的函数可以使用fetch.
```
function sendRequest(url: string[],max: number,callback: ()=>void);
```

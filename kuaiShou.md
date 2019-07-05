1. 请写出一下代码执行结果。
```
var a = {x: 1}
var b = a;
a.x = a = {n: 1};
console.log(a);
console.log(b);
```

2. 请写出以下代码执行结果
```
Function.prototype.a = ()=> alert(1);
Object.prototype.b = () => alert(2);
function A(){};
const a = new A();
a.a();
a.b();
```
3. 请写出以下代码执行结果
```
let a = 0;
console.log(a);
console.log(b);
let b = {};
console.log(c);
function c() {};
```

4. 请写出以下代码执行结果
```
var x = 10;
function a(y) {
  var x = 20;
  return b(y);
}
function b(y) {
  return x+y;
}
a(20);
```

5. 请写出以下代码执行结果
```
console.log(1);
setTimeout(()=> {
  console.log(2)
});
process.nextTick(()=> {
  console.log(3);
});
setImmedite(()=> {
  console.log(4);
});
new Promise(resolve=> {
  console.log(5);
  resolve();
  console.log(6);
  }).then(()=> {
    console.log(7);
});
Promise.resolve().then(()=> {
  console.log(8);
  process.nextTick(()=> {
    console.log(9);
    })
})
```

6. 请写出以下代码执行结果
```
[1,2,3,4,5].map(parseInt);
```

7. 请写出以下代码执行结果
```
typeof typeof typeof [];
```
8. 以下CSS最后是什么颜色
```
<style>
div {color: red};
#title {color: yellow};
div.title {color: blue};
</style>
<div class="title" id="title">abc</div>
```
9. 以下CSS最后是什么颜色？
```
<style>
.classA {color: blue}
.classB {color: red}
</style>
<p class="classB classA">123</p>
```

10. 请解释一下什么BFC，IFC，FFC。

11. visibility: hidden 和 display: none 有什么区别？

12. css中你所知道的长度单位有哪些？有哪些区别？

13. img 的 alt 和 title有何不同

14. 你如何理解a11y?

15. 请解释一下Node中垃圾回收算法主要有哪些，分别使用在什么场景。

16. 什么是死锁，以及死锁产生的必要条件有哪些？

17. 请实现一个算法，实现数组乱序，要求每个数字出现在每个位置的概率是平均的。


18. 请补充一下代码

```
function add() {};
function one() {};
function two() {};
console.log(one(add(two())));//3
console.log(two(add(one())));//3
```

19. 请实现一个cacheRequest方法，保证当前ajax请求相同资源时，真实网络层中，实际只发出一次请求（假设已经存在request方法用于封装ajax请求，调用格式为request(url, successCallback, failCallback)）比如调用方代码如下：

```
//a.js
cacheRequest('/user',data=> {
  console.log('我是从A请求的user, 数据为'+ data);
})
```

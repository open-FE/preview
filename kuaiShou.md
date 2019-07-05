
1.请写出已下代码的执行结果
 ```
 var a = {x:1};
 var b = a;
 a.x = a = {n: 1};
 console.log(a);
 console.log(b);
 ```
2.请写出以下代码的执行结果
```
Function.prototype.a = ()=> alert(1);
Object.prototype.b = ()=> alert(2);
function A(){};
const a = new A();
a.a();
a.b();
```
3.请写出以下代码执行结果
```
let a = 0;
console.log(a);
console.log(b);
let b = 0;
console.log(c);
function c(){}
```

# test
面试题？

```js
var a = [];
var c = [1,2,3]; 
for ( i in c ){
  a[i] = function (){
    return c[i];
    }
} 
while(d = a.pop())
console.log(d());//2 2 2
```
for( i in arr ) 中的i为下标 

function(){ return i } 中的i是对循环中i的引用。所以为最终值。

```
var str='abc123'; 
var num=parseInt(str); 
if(num==NaN){alert(NaN);} 
else if(num==123){alert(123);} 
else if(typeof num=='number'){alert('number');} 
else{alert('str');}
```
这些代码输出的结果是（）？

正确答案 alert('number');

parseInt();首先查看位置0处的字符，判断它是否是个有效数字；如果不是，该方法将返回NaN，不再继续执行其他操作。

但如果该字符是有效数字，该方法将查看位置1处的字符，进行同样的测试。这一过程将持续到发现非有效数字的字符为止，

此时parseInt()将把该字符之前的字符串转换成数字。此外NaN==NaN为false,typeof NaN=='number'为true。

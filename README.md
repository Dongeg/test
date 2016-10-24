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

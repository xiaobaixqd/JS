# 解释代码
* 
``` javascript
let i=0
for(i=0;i<6;i++){
    setTimeout(()=>{
        console.log(i)
    },0)
}
```
* setTimeout不是立马执行的，因为 js 是单线程的，有一个事件队列机制，setTimeout的回调会到了延迟时间塞入事件队列中，排队执行。

# 写出让上面代码打印 0、1、2、3、4、5 的方法
* 
``` javascript
for(let i=0;i<6;i++){
    setTimeout(()=>{
        console.log(i)
    },0)
}
```

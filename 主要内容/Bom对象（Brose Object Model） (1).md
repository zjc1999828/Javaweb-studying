![在这里插入图片描述](https://img-blog.csdnimg.cn/dcdb1d64fccd4398a91f1a00e4241fab.png?x-oss-process=image/watermark,type_d3F5LXplbmhlaQ,shadow_50,text_Q1NETiBATkpVU1RaSkM=,size_20,color_FFFFFF,t_70,g_se,x_16)
![在这里插入图片描述](https://img-blog.csdnimg.cn/5ed49cf8241e4fe88f25215cf6dd86f4.png?x-oss-process=image/watermark,type_d3F5LXplbmhlaQ,shadow_50,text_Q1NETiBATkpVU1RaSkM=,size_20,color_FFFFFF,t_70,g_se,x_16)


==confirm()注意点:==
confirm()函数具有返回值，点击确定返回true，点击取消返回false。






==setInterval注意点:==
一定要用function(){}将调用的函数包裹起来放在setInterval中才可以实现效果
```javascript
var a = 1;
var b = 2;
function sd(a,b){
    alert(a+b)
}
window.setInterval(function () {
    sd(1,2)
},2000)

```


# 获取HTML对象的方式
----
----

![在这里插入图片描述](https://img-blog.csdnimg.cn/0ca8f24960ea428ba02b13f7bb8df7bf.png?x-oss-process=image/watermark,type_d3F5LXplbmhlaQ,shadow_50,text_Q1NETiBATkpVU1RaSkM=,size_20,color_FFFFFF,t_70,g_se,x_16)

注意2/3/4方式返回的是数组。因为id是唯一的。


#### 常见的适用于所有对象的方法：
1. innerhtml改变内容

![在这里插入图片描述](https://img-blog.csdnimg.cn/b03d8916a96c410d8ca4942ae133faeb.png?x-oss-process=image/watermark,type_d3F5LXplbmhlaQ,shadow_50,text_Q1NETiBATkpVU1RaSkM=,size_20,color_FFFFFF,t_70,g_se,x_16)


2. 对于复选框的checked属性。![在这里插入图片描述](https://img-blog.csdnimg.cn/359e8a43bdf04036b2432b0d81bd8a06.png)

3. style改变css的样式
![在这里插入图片描述](https://img-blog.csdnimg.cn/0942b56dd5394e888619e28f6702cafd.png?x-oss-process=image/watermark,type_d3F5LXplbmhlaQ,shadow_50,text_Q1NETiBATkpVU1RaSkM=,size_20,color_FFFFFF,t_70,g_se,x_16)
4. 对于Img对象
img.src是改变图片源的。

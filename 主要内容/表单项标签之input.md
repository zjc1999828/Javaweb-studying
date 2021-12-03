# 表单项标签之input
----
----


![在这里插入图片描述](https://img-blog.csdnimg.cn/ef38d7e5b5b244b49fa9b095e77ee9fd.png?x-oss-process=image/watermark,type_d3F5LXplbmhlaQ,shadow_50,text_Q1NETiBATkpVU1RaSkM=,size_20,color_FFFFFF,t_70,g_se,x_16)


```xml

<body>
<form action="#" method="post">


    <input type="hidden" name="id" value="123">
    <label for="username">用户名:</label> <input type="text" name = "username" id="username"><br>

    <label for="password">密码:</label> <input type="password" name="password" id="password"><br>

    <label for="male">男:</label><input type="radio" name="gender" id="male" value="1">
    <label for="female">女:</label><input type="radio" name="gender" id="female" value="2"><br>
    <label for="旅游">旅游:</label><input type="checkbox" name="tourtype" id="旅游" value="1"><br>
    <label for="游戏">游戏:</label><input type="checkbox" name="tourtype" id="游戏" value="2"><br>
    <label for="洗澡">洗澡:</label><input type="checkbox" name="tourtype" id="洗澡" value="3"><br>
    <label >文件上传:</label><input type="file" ><br>


    <input type="submit" value="提交"><br>
    <br>
    <input type="reset" value="重置"><br>
    <br>
    <input type="button" value="2321">

</form>
```


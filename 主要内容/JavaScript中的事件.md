![在这里插入图片描述](https://img-blog.csdnimg.cn/9b2f46483f334cf59acdb4894aae62e0.png?x-oss-process=image/watermark,type_d3F5LXplbmhlaQ,shadow_50,text_Q1NETiBATkpVU1RaSkM=,size_20,color_FFFFFF,t_70,g_se,x_16)


常见的事件功能：
1. onblur失去焦点



2. onfoucs获得焦点


3. onmouseover鼠标移到某个元素之上


4. onmouseout鼠标移开某个元素



5. onsubmit 表单验证常用按钮
==表单验证的例子==
![在这里插入图片描述](https://img-blog.csdnimg.cn/c2d80e3aecc648dd93475785deb2ef83.png?x-oss-process=image/watermark,type_d3F5LXplbmhlaQ,shadow_50,text_Q1NETiBATkpVU1RaSkM=,size_20,color_FFFFFF,t_70,g_se,x_16)

onsubmit返回true，表单提交
onsubmit返回false，表单不提交


例子:

```javascript
<!DOCTYPE html>
<html lang="en">
<head>

    <meta charset="UTF-8">
    <title>Title</title>
</head>



<body>

<form id="registerform" action="#" method="get">

    <input type="hidden" name="id" value="123">
    <label for="username">用户名:</label> <input type="text" name = "username" id="username"><br>
    <span id="usernameerror" name="usernameerror">用户名不符合规则样式</span><br>


    <label for="password">密码:</label> <input type="text" name="password" id="password"><br>
    <span id="passworderror" name="passworderror">密码不符合规则样式</span><br>

    <label for="phonenumber">手机号:</label><input type="text" name="phonenumber" id="phonenumber"><br>
    <span id="phonenumbererror" name="phonenumbererror">手机号不符合规则样式</span><br>


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
    <input type="button" value="2321"><br>
    <br>

    <label>城市选择:</label>
    <select name="city">
        <option>北京</option>
        <option>上海</option>
        <option>南京</option>
        <option>佛山</option>
    </select>
    <br>
    <br>


    <label>个人描述:</label>
    <textarea name="description" rows="5" cols="5">
    </textarea>
</form>


<script >
var usernameerror = document.getElementById("usernameerror");
usernameerror.style.display="none";
var username = document.getElementById("username");
username.onblur = checkusername;
function checkusername(){
    var flag = username.value.trim().length>6 && username.value.trim().length<12;
    if(username.value.trim().length>6 && username.value.trim().length<12){
        usernameerror.style.display="none";
    
    }
    else{
        usernameerror.style.display="";
    }
    return flag
}







var passworderror = document.getElementById("passworderror");
passworderror.style.display="none";

var password = document.getElementById("password");
password.onblur = checkpassword;
function checkpassword(){
    var flag = password.value.trim().length>6 && password.value.trim().length<12;
    if(password.value.trim().length>6 && password.value.trim().length<12){
        passworderror.style.display="none";

    }
    else{
        passworderror.style.display="";
    }
    return flag
}




var phonenumbererror = document.getElementById("phonenumbererror");
phonenumbererror.style.display="none";

var phonenumber = document.getElementById("phonenumber");
phonenumber.onblur = checkphonenumber;
function checkphonenumber(){
    var flag = phonenumber.value.trim().length>6 && phonenumber.value.trim().length<12;
    if(phonenumber.value.trim().length>6 && phonenumber.value.trim().length<12){
        phonenumbererror.style.display="none";

    }
    else{
        phonenumbererror.style.display="";
    }
    return flag
}

var registerform = document.getElementById("registerform");
registerform.onsubmit = checksubmit;
function checksubmit(){
    return checkpassword()&&checkphonenumber()&&checkusername();
}

</script>


</body>



</html>
```


### js笔记
基础 ：chrom控制台 win：ctrl shift j  
## *前期在控制台写代码*
1. 变量容器var：var a = 1；var name = "will 
2. alert() 弹窗显示
3. prompt（）弹窗输入
```javascript
var name = prompt("请输入您的姓名："); 
var gender = prompt("请输入您的性别："); 
var age = prompt("请输入您的年龄："); alert("姓名"+name);
```
-----变量结束------   

## *选择流程*
if（...）{...}-- else if（...）{...}---else{...}  
转义字符 \
```javascript
var name = prompt("请输入您的姓名：");
var gender = prompt("请输入您的性别："); 
var age = prompt("请输入您的年龄："); 
alert("姓名"+name);
if(age>18){
	alert("你已通过年龄验证！")
}
else if(age<18){
	alert("未成年！")
}
else{
	alert('18!')
	};
```
------选择流程结束------

## *函数*
加载js  
1.<script></script>标签内书写
<!--放在网页文件最后编写，因为浏览器一行行实时渲染，放在body后会先加载网页·让人感觉不卡顿-->
2.<script src = "....js"></script>外部加载

3.函数---功能代码
   创建--->调用--->生效

​	*3.1创建*  
​			function 函数名（参数）{
​				函数体；
​				return；							}
​	*3.2调用*  
​			函数名（参数值）；
*函数    DRY原则 不要重复造轮子*
Do not repeat yourself
<!------- return执行，函数结束。（所以两个return没得用）--------->

```javascript
function jiaFa(a,b){
    return a+b;
}
alert(jiaFa(1,2));
```
-----------函数结束-------------

## *数组*
1.数组是特殊变量
2.var 数组名 = ['','','']
3.数组中可以存入函数，可存万物
4.数组名[函数名]（）-----调用


*------数组方法------*
.shift() 切出第一项
.pop() 切出最后一项
.forEach( function(value,index) {
遍历数组获取值与索引；新方法旧浏览器慎用
} )

*--------循环loops-----------*
1.while （）{} 为真循环
do {} while（）先执行一次再判断条件

2.for（ *setup初始定义变量；comparsion变量限定条件；change变量变换语句* ）

{ 循环语句} 
<!--console.log()控制台打印-->

## ------------DOM操作--------------

document

1. document.getElementsByTagName('')[第几个标签]  
   获取html内标签
   var pTags = document...变量操作

2. document.getElementsByClassName
   document.getElementsById
   document.querySelector('.')匹配的第一个类名
   document.querySelector('#'匹配的)第一个id
   document.querySelectorAll('')所有匹配元素

3. firstPTag = document.querySelector('p') 第一个p元素
   firstPTag.innerHTML =  "操作语句"

4. var li = document.querySelector('类名')  
   类操作
   li.className = "" 类名重命名
   li.className = li.className + "" 类名结尾添加
   li.className = li.className.replace("","") 替换类名

5. li.classList 显示所有类名
   li.classList.new('')
   li.classList.remove('')

6. li 定位li元素
   li.parentElement li的父亲
   li.parentElement.children[]




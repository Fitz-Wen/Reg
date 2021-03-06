##  正则表达式

### 规则
```
\b	   		匹配一个字边界，即字与空格间的位置
\d     		一个数字
\w     		一个字母或数字
\s     		可以匹配一个空格（也包括Tab等空白符）
.      		任意一个字符
*           任意个字符（包括0个）
+           表示至少一个字符
?           表示0个或1个字符 
{n}    		表示n个字符
{n,m}  		表示n-m个字符
A|B    		可以匹配A或B
^      		表示行的开头
$      		表示行的结束
[a-z]  		匹配所有的小写字母 
[A-Z]  		匹配所有的大写字母 
[a-zA-Z] 	匹配所有的字母 
[0-9]    	匹配所有的数字 
[0-9\.\-] 	匹配所有的数字，句号和减号 
```
###  常用正则
```
数字：^[0-9]*$
n位的数字：^\d{n}$
至少n位的数字：^\d{n,}$
m-n位的数字：^\d{m,n}$
汉字: /^[\u2E80-\u9FFF]+$/
Email地址：/^\w+([-+.]\w+)*@\w+([-.]\w+)*\.\w+([-.]\w+)*$/
身份证号(15位、18位数字)，最后一位是校验位，可能为数字或字符X： (^\d{15}$)|(^\d{18}$)|(^\d{17}(\d|X|x)$)
```

# Python
## Resource 
ANACONDA Python 
MongoDB Community Edition
### 24th June
str='Runoob'
|                       |                         |
| ---------------------:|------------------------:|
|print(str)      |# 输出字符串              | 
|print(str[0:-1])|# 输出第一个到倒数第二个的所有字符  | 
|print(str[0])   |# 输出字符串第一个字符 | 
|print(str[2:5]) |# 输出从第三个开始到第五个的字符 | 
|print(str[2:])  |# 输出从第三个开始后的所有字符| 
|print(str * 2)  |# 输出字符串两次 | 
|print(str + '你好') |# 连接字符串| 
|print('hello\nrunoob')| # 使用反斜杠(\)+n转义特殊字符 | 
|print(r'hello\nrunoob')|# 在字符串前面添加一个 r，表示原始字符串，不会发生转义 | 
### 25th June Input
```
input("\n\n按下 enter 键后退出。")
```
```
name = input("What's your name? ")
print("Nice to meet you " + name + "!")
age = input("Your age? ")
print("So, you are already " + age + " years old, " + name + "!")
```
### 26th June Several ; in one row
```
import sys; x = 'runoob'; sys.stdout.write(x + '\n')
```
print without changing row: end=""
```
x="a"
y="b"
# 换行输出
print( x )
print( y )
 
print('---------')
# 不换行输出
print( x, end=" " )
print( y, end=" " )
print()
```
### 27th June import
import somemodule
from somemodule import somefunction
from somemodule import firstfunc, secondfunc, thirdfunc
from somemodule import *
```
import sys
print('================Python import mode==========================')
print ('命令行参数为:')
for i in sys.argv:
    print (i)
print ('\n python 路径为',sys.path)
```
```
from sys import argv,path  #  导入特定的成员
 
print('================python from import===================================')
print('path:',path) # 因为已经导入path成员，所以此处引用时不需要加sys.path
```
### 28th June Data Type in Python 3
```
a,b,c,d=10, -5.5, True, 4+4j
print(type(a),type(b),type(c),type(d))
```
```
a=111
isinstance(a,int);
```
The difference between type() and isinstance()
```
>>> class A:
...     pass
...
>>> class B(A):
...     pass
...
>>> isinstance(A(),A)
True
>>> type(A())==A
True
>>> isinstance(B(),A)
True
>>> type(B())==A
False
```
```
>>> 5+4
9
>>> 4.3-2
2.3
>>> 3*7
21
>>> 2/4
0.5
>>> 2//4 get integer
0
>>> 17%3 #remainder
2
>>> 2**5
32




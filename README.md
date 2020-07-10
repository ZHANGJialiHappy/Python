# Python
https://www.runoob.com/python3/python3-data-type.html
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
Data type which can't be changed: Number, String, Tuple. 
Data type which can be changed: list, Dictionary, Set
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
```
```
>>> m=[1,2,3,4,5,6]
>>> m[0]=9
>>> m[2:4]=[12,13]
>>> m[4]=5//3
>>> m[5]=19%5
>>> m[1]=2**3
>>> m
[9, 8, 12, 13, 1, 4]
>>> m[2:5]=[]
>>> m
[9, 8, 4]
```
### 29th June Tuple, Set and Dictionary
tuple uses ()
```
tuple=('abc', 786)
tup1=()
tup2=(20,)
```
set uses {} or set()
```
>>> sites={'Google', 'Taobao', 'Runoob', 'Facebook', 'Zhihu', 'Baidu'}
>>> print(sites)
{'Zhihu', 'Facebook', 'Baidu', 'Runoob', 'Google', 'Taobao'}
>>> if 'Runoob' in sites:
...     print('Runoob is in the set')
... else:
...     print('Runoob is not in the set')
...
Runoob is in the set
>>> a=set('asdfghhj')
>>> b=set('ascfgb')
>>> print(a)
{'h', 'g', 'f', 's', 'd', 'j', 'a'}
>>> print(a-b)
{'j', 'h', 'd'}
>>> print(a|b)
{'c', 'h', 'g', 'f', 's', 'b', 'd', 'j', 'a'}
>>> print(a&b)
{'a', 'f', 'g', 's'}
>>> print(a^b)
{'c', 'h', 'd', 'j', 'b'}
```
Dictionary
```
>>> dict={}
>>> dict['one']="1-education"
>>> dict[2]="2-tool"
>>> tinydict={'name':'runoob','code':1, 'site': 'www.runoob.com'}
>>> print(dict['one'])
1-education
>>> print(dict[2])
2-tool
>>> print(tinydict)
{'name': 'runoob', 'code': 1, 'site': 'www.runoob.com'}
>>> print(tinydict.keys())
dict_keys(['name', 'code', 'site'])
>>> print(tinydict.values())
dict_values(['runoob', 1, 'www.runoob.com'])
```
### Operator
+ - * / % ** //
```
>>> a=21
>>> b=10
>>> c=0
>>> print("1-c=" +str(c))
1-c=31
>>> c=a-b
>>> print("2_c+" + str(c))
2_c+11
>>> print("2_c=" + str(c))
2_c=11
>>>
>>> c=a+b
>>> print("c1="+str(c))
c1=31
>>> c=a-b
>>> print("c2="+str(c))
c2=11
>>> c=a*b
>>> print("c3="+str(c))
c3=210
>>> c=a/b
>>> print("c4="+str(c))
c4=2.1
>>> c=a%b
>>> print("c5="+str(c))
c5=1
>>> c=a//b
>>> print("c6="+str(c))
c6=2
>>> # change variable
... a=2
>>> b=3
>>> c=a**b
>>> print("c7="+str(c))
c7=8
```
== != > < >= <=
```
>>> if(a==b):
...     print("a=b")
... else:
...     print("a!=b")
...
a!=b
>>> if(a>b):
...     print("a>b")
... else:
...     print("a<=b")
...
a>b
```
+= -= *= /= %= **= //= :=(after Python3.8)
```
>>> a=21
>>> b=10
>>> c=0
>>> c=a+b
>>> print("c1="+ str(c))
c1=31
>>> c+=a # c=c+a
>>> print("c2="+ str(c))
c2=52
>>> c-=a #c=c-a
>>> print("c3="+str(c))
c3=31
>>> c*=a # c=c*a
>>> print("c4="+ str(c))
c4=651
>>> c/=a #c=c/a
>>> print("c5="+ str(c))
c5=31.0
>>> c=2
>>> c%=a
>>> print("c6="+ str(c))
c6=2
>>> c**=a
>>> print("c7="+ str(c))
c7=2097152
>>> c//=a
>>> print("c8="+ str(c))
c8=99864
```
in, not in
```
>>> a=10
>>> b=20
>>> List=[1,2,3,4,5]
>>> if (a in List):
...     print("a is in the list")
... else:
...     print("a is not in the list")
...
a is not in the list
>>> a=2
>>> if (a in List):
...     print("a is in the list")
... else:
...     print("a is not in the list")
...
a is in the list
```
& | ^ ~ << >>
```
>>> a=60
>>> b=13
>>> c=0
>>> c=a&b; #	按位与运算符：参与运算的两个值,如果两个相应位都为1,则该位的结果为1,否则为0
>>> print("c1=" + str(c))
c1=12
>>> c=a|b # 按位或运算符：只要对应的二个二进位有一个为1时，结果位就为1。
>>> print("c2=" + str(c))
c2=61
>>> c=a^b # 按位异或运算符：当两对应的二进位相异时，结果为1
>>> print("c3=" + str(c))
c3=49
>>> c=~a # 按位取反运算符：对数据的每个二进制位取反,即把1变为0,把0变为1。~x 类似于 -x-1
>>> print("c4=" + str(c))
c4=-61
>>> c=a<<2 # 左移动运算符：运算数的各二进位全部左移若干位，由"<<"右边的数指定移动的位数，高位丢弃，低位补0。
>>> print("c5=" + str(c))
c5=240
>>> c=a>>2 # 右移动运算符：把">>"左边的运算数的各二进位全部右移若干位，">>"右边的数指定移动的位数
>>> print("c6=" + str(c))
c6=15
```
is is not
```
>>> a=20
>>> b=20
>>> if(a is b): # id(a)==id(b)
...     print("a is the same with b")
...
a is the same with b
>>> a=10
>>> if (a is not b):
...     print( "a is not the same with b")
...
a is not the same with b
```
and or not

### 30th June Number Type
Int, float, complex
在交互模式中，最后被输出的表达式结果被赋值给变量 _ 
```
>>> tax=12.5/100
>>> price=100.50
>>> price*tax
12.5625
>>> price+_
113.0625
>>> round(_,2)
113.06
```
String 
```
>>> var1="Hello World!"
>>> var2="Runoob"
>>> print("updated string:", var1[:6]+var2)
updated string: Hello Runoob
```
### 10th July 
string
```
>>> print("I am %s, and I am %d years old" %('Jiali',30))
I am Jiali, and I am 30 years old
```
```
>>> str="""in three quotation marks, we can use
... TAB(\t).
... We can also use[\n].
... """
>>> print(str)
in three quotation marks, we can use
TAB(	).
We can also use[
].
```
List
```
>>> a=[1,2,3]
>>> b=['a','b','c']
>>> c=[a,b]
>>> c[0]
[1, 2, 3]
>>> c[0][1]
2
```



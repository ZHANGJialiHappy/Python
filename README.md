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
Data type which can't be changed: Number, String, Tuple
Data tyoe which can be changed: list, Dictionary, Set
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


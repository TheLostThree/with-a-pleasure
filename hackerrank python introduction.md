## introduction
#### mod divmod
##### divmod(a,b)
例子：
```
>>>print divmod(177,10)    
(17,7)  # a代表整除数，b代表余数
```
```python
from __future__ import division
a = int(raw_input())
b = int(raw_input())
print a//b  # 代表整数除法
print a%b  # 代表取余数
print divmod(a,b) #得到整除数和余数
```

#### mod power
##### pow(a,b,m)
例子：
```
>>> pow(a,b)  # a为底数，b为底数
>>>a**b     # 同上
>>>pow(a,b,m)  # a,b代表a^b，m代表除数,输出的结果是得到的余数
```
```python
a = int(raw_input())
b = int(raw_input())
m = int(raw_input())
print pow(a,b)
print pow(a,b,m)
```

#### interchange two numbers
这题要求用tuple做，其实就只是调换两个数值的顺序。  
```python
a = raw_input()
b = raw_input()
mytuple = (b,a) # 其实就是tuple赋值时，先弄好顺序。
print mytuple[0]
print mytuple[1]
```

#### finding the percentage
这题好像不适合用在introduction里的。   
输入学生人数，再输入学生名字和三门课分数，最后通过输入学生名字查到三门的平均分。
```python
stu_number = int(raw_input())
mydict={}
for i in range(stu_number):
    info = raw_input().split(' ')
    score = map(float,info[1:])
    mydict[info[0]] = sum(score)/float(len(score))
print '%.2f' %mydict[raw_input()]
```

#### print function
这个应该是python3中print变成函数后的功能。
```python
from __future__ import print_function
for i in range(1, int(raw_input())+1):  # sep代表数值之间的分隔符，end代表打印完数值之后的字符
    print (i, sep='', end='')
>>>print(value, ..., sep=' ', end='\n', file=sys.stdout) #p新版本中print的函数
```




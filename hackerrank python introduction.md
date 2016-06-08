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





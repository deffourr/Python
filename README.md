# Python
В библиотеке **Collections** есть множество полезных функций. Например, Counter: 
```python
from collections import Counter
print(Counter("aaabbbcccd"))
>>> Counter({'a' : 3, 'b' : 3, 'c' : 3, 'd' : 1})
```
**icecream** отлично подходит для отладки кода:
```python
from icecream import ic 

num1 = 30
num2 = 40 

ic(num1)
ic(num2)
>>> ic| num1: 30
>>> ic| num2: 40

```

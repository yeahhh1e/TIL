### string과 int/float 같은 줄에 출력하는 방법
```python
1.
print(f"One third, expressed as a float is: {1 / 3}")
# 'One third, expressed as a float is: 0.3333333333333333'

2.
# 원주율
pie = 3.1415926535897932384626433832795028841971693993751058209749445923078164062862089986280348253421170679
# 반지름
circle = 15
circle_3 = '원의 둘레 : '

print(f"{circle_3}"f"{circle*2*pie}")
# 원의 둘레 : 94.24777960769379
```

### 연산자 우선순위


| 우선순위 | 연산자         | 연산                   |
|:----:|:-----------:|:--------------------:|
| 높음   | **          | 지수                   |
|      | -           | 음수 부호                |
|      | *, /, //, % | 곱셈, 나눗셈, 정수 나눗셈, 나머지 |
| 낮음   | +, -        | 덧셈, 뺄셈               |



출처 : https://realpython.com/how-to-python-f-string-format-float/


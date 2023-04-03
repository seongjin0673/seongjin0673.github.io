---
layout: post
title:  "1주차 python 기초 1"
---

#  01. Python Basic 01

# 실습 목표
1. 데이터 타입을 알고 있다. - 숫자,문자,boolean
2. 제어문을 사용할 수 있고, 제어문이 사용된 소스코드를 이해할 수 있다.
3. 리스트(List)를 이해하고, 리스트가 사용된 소스코드를 이해할 수 있다. 리스트를 사용할 수 있다.
4. 함수(Function)가 무엇인지 알고, 함수가 사용된 소스코드를 이해할 수 있따. 간단한 함수를 작성할 수 있다.

 print("Hello, Python World!!")
  
  Hello, Python World!!

 print("파이썬 기초")

  파이썬 기초


a = 3
print(a) #a 를 출력한다
type(a) #a의 Type을 출력한다.

3
int

a = 'ab'
print(a)
type(a)

ab
str

# 변수 할당

midterm = 65
final = 90
quiz = 99

print(quiz)

results = midterm*0.4 + final*0.4 + quiz*0.2
print(results)

99
81.8

# 다중 할당
midterm, final, quiz = 65, 90, 99

results = midterm*0.4 + final*0.4 + quiz*0.2
print(results)

81.8

# 3. Type & Operator - Number
- number: int, float
- 산술 연산자

# 학점 규칙: 중간고사 40%, 기말고사 40%, 퀴즈 20%
print(type(midterm))
print(results)
print(type(results))

<class 'int'> #midterm의 class 출력
81.8  #이전에 할당한 results 출력
<class 'float'> #자동으로 float로 지정


# float
a = 10/3
print(a)
print(type(a))

3.3333333333333335 # 10/3 계산을 한 a를 출력
<class 'float'> # a의 calss 출력

# complex (제곱 후에 -1이 되는 수를 j라고 한다)
comp_01 = complex(3,5) 
comp_02 = 3 + 5j
print(comp_01)
print(comp_02)
print(type(comp_01))
print(type(comp_02))

(3+5j) #
(3+5j)
<class 'complex'>
<class 'complex'>

# 수리 연산자
+, -, *, /
%
**
//
+=, -=, *=, /=

10/7 #나머지값을 출력한다.

값 : 1.4285714285714286

10//7 # 몫의 값을 출력한다.

값 : 1 

print(1,2,3)

값 : 1 2 3

print('1\t2\t3') #출력할 값들의 중간에 탭이 들어가서 띄어쓰기 된다.

값 : 1	    2   	3

print(1,2,3,sep='\t') ( sep를 사용해서 아래로 출력되도록 설정)

값 : 1
     2
     3


print(3,end='\t*\t\n') # 3이 끝날때는  탭과 *을 출력
print(5,end='*') #5가 끝날때는 *이 출력










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


# 4. Type & Operator - String
-string
-print 활용


# 문자열
# 파이썬은 문자열에 대해 상당한 편의성을 지원합니다.

thanks = 'thanks'
name = '실무데이터분석'
tn = thanks +',    '+ name # 4칸을 띄어쓰면, 동일하게 4번 나옵니다.

print(tn)
print(len(thanks))
print(len(name))
print(len(tn))

thanks,    실무데이터분석 # thanks + '    '+name인 실무데이터 분석이 출력됩니다.
6   #len 함수는 수를 나타냅니다
7   #len 함수는 수를 나타냅니다
18   #len 함수는 수를 나타냅니다


# multi line string """으로 시작하고 끝나는 구간은 모두 문자 변수
multilines = """
hello, python world
- keras
- anything
"""
print(multilines)


hello, python world
- keras
- anything


print('여기에 %d 을 출력하고싶다' % (5)) #뒤에서 오는 값을 할당해줍니다.

여기에 5 을 출력하고싶다

print('여기에 %s을 출력하고싶다' % ('5입니다.'))
여기에 5입니다.을 출력하고싶다


# 5. Container - List
list
add & remove

#name, midterm, final, quiz = "Geoffery Hinton", 95, 65, 90
#stu02 - name, midterm, final, quiz = "Yann Lecun", 80, 85, 90
#stu03 - name, midterm, final, quiz = "Yoshua Bengio", 92, 88, 84
#stu04 - name, midterm, final, quiz = "Andrew Ng", 75, 85, 100

# 리스트 생성
stu01 = ["Geoffery Hinton", 95, 65, 90]
stu02 = ["Yann Lecun", 80, 85, 90]
stu03 = ["Yoshua Bengio", 92, 88, 84]
stu04 = ["Andrew Ng", 75, 85, 100]

print(type(stu01))

<class 'list'> # class가 생성된다.

print(stu03) 

['Yoshua Bengio', 92, 88, 84] # stu03의 리스트가 출력됩니다.

print(stu03[0]) 
Yoshua Bengio #stu03 리스트의 0번째 원소인 Yoshua Bengio가 출력됩니다.

# 2차원 리스트
stu = [stu01, stu02, stu03, stu04]
stu = [["Geoffery Hinton", 95, 65, 90], stu02, stu03, stu04]

print(type(stu01)) # 2차원 리스트를 통해서 stu01 을 stu의 중간에 위치시킨다.




# list 자세히

l = [1,2]
print(l)
print(type(l))

[1, 2] #l 에 있는 리스트가 출력된다.
<class 'list'> # l번의 클래스인 list 가 출력 된다.


print(l[0], l[1], sep='\n') # l 번의 0 번째 원소와 1번째 원소를 출력한다(sep='\n'을 통해서 줄바꿈)
1
2


ts= [1, 2, ['a', 'b']]
print(ts)

[1, 2, ['a', 'b']] #ts의 리스트가 출력된다.


print(ts[2][0]) #ts 리스트의 3번째 리스트 안에 있는 첫번째 원소가 출력된다.

a # a가 출력

# 리스트 추가, 제거
#stu01 - name, midterm, finals, quiz = "Geoffery Hinton", 95, 65, 90
#stu02 - name, midterm, final, quiz = "Yann Lecun", 80, 85, 90
#stu03 - name, midterm, final, quiz = "Yoshua Bengio", 92, 88, 84
#stu04 - name, midterm, final, quiz = "Andrew Ng", 75, 85, 100

#리스트 생성
stu01 = ["Geoffery Hinton", 95, 65, 90]
stu02 = ["Yann Lecun", 80, 85, 90]
stu03 = ["Yoshua Bengio", 92, 88, 84]
stu04 = ["Andrew Ng", 75, 85, 100]


## 요소 추가하기 
print(stu01)
stu01.append(100) # append를 사용하여 stu01 리스트 맨 마지막에 100이라는 원소를 추가한다.
print(stu01)

['Geoffery Hinton', 95, 65, 90] # 추가 전
['Geoffery Hinton', 95, 65, 90, 100] #추가 후


## 요소 제거하기 
print(stu01)
del stu01[0] # stu01이라는 리스트의 0번째 원소를 제거 한다.
print(stu01)

['Geoffery Hinton', 95, 65, 90, 100] # 제거 전
[95, 65, 90, 100] # 제거 후


## 요소 변경하기
print(stu01)
stu01[0] = 99 # stu01 리스트 안에 있는 0번째 원소를 99로 변경한다.
print(stu01)



a='this is sentence'
# a 에서 "is" 만을 출력하시오
result =a[5:7] # 5번째부터 7번째까지 result로 지정
print(result) # 지정한 result값을 출력














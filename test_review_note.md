---
marp: true
theme: cover
class: invert
paginate: true
header: Marp tutorial
footer: 2023-02-10
---

<!--_color: orange-->

# _<!--fit-->C# TEST REVIEW!_

by. programers

---

# 코딩 테스트 활용법 by. 요기요개발자

## 1. 습관 만들기
- 하루에 딱 한 문제만 푼다.
- 대신에 매일매일 한다.
- 모르는 문제가 나오면 고민을 해보고, 1시간이 넘어간다 싶으면 답을 본다.
- 답을 보고 내 코드를 비교해보고, 회고를 해본다.

---

## 2. 유형분석 & 유형별 풀이

- 1번이 익숙해지면 쉬운 유형 문제부터 진행한다.
- 답이 맞고 틀리기에 집착한다기 보다는 어떤 유형이 있는지 파악한다.

---

## 3. 난이도 올리기

- 쉬운 유형에 어느정도 익숙해지면 조금씩 난이도를 올린다.

4. 매일매일 꾸준히 계속 풀기

- 1~4의 과정을 매일매일 반복하면서 조금씩 꾸준히 푼다.

5. 매일 푸는 문제들을 다른 사람들의 코드와 비교해서 어떤 점을 개선할 수 있을지 스스로 회고해 본다.

---

## Action Items

1. 코딩 테스트 사이트 1개를 정하고 오늘 바로 내 수준에 맞는 혹은 더 낮은 '1'문제를 푼다. 이것을 매일매일 실천해 본다.

2. 자체 코딩 테스트를 치르고, 공개되어 있는 회사들의 문제들을 보고 어떤 유형이 나오는지 파악해본다.

3. 내가 푼 문제를 글로 남기고, **개선점**을 회고해 본다.

---

- ## 소수점 나눗셈 (반올림) 문제 회고록

``` c#
using System;

public class Soulution {
    public double solution (double num1, double num2) {

        double answer = Math.Truncate (num1/num2*1000);
        return answer;
    }
}
```
변수 int 대신에 double을 넣어준다
: int를 변수로 넣으면 정수 값만 나오기 때문에
Math.Round 를 넣어서 소수점 뒷자리를 없애준다. 

자세한 내용 참고 : https://cosmosproject.tistory.com/529

---

## 반올림/ 올림/ 내림? 

-Math.Round(인자값): 반올림 : 소수점 반올림??

-Math.Ceiling(인자값): 올림 : 소수점을 올림한 수

-Math.Floor(인자값): 내림 : 소수점 뒤의 숫자를 모두 지움.

![](./test_review_note/mathround.jpg)

---

## 나머지 구하기

-숫자와 숫자 사이에 '%' 를 사용.--> 몫만 알 수 있음.

![](./test_review_note/save_namergi.jpg)


참조링크: https://learn.microsoft.com/ko-kr/dotnet/csharp/language-reference/operators/arithmetic-operators

---

## 배열의 평균값

- 배열 관련 메서드

Name.Max() : 배열 요소 중 최대값 반환.

Name.Min() : 배열 요소 중 최소값 반환.

Name.Sum() : 배열 요소의 합계 반환.


참조링크: https://homzzang.com/b/cs-20



---

## - class의 특징?
모든 클래스는 **복합 데이터** 형식이다. 
복합데이터 형식은 참조 형식이다.
<br>
```c#
Cat kitty = new cat();
```
<br>
kitty는 'null'을 가진다.
kitty 자체에 메모리가 할당되는 것이 아니라, 참조로서 객체가 있는 곳을 가리킨다.

---

new : 연산자

역할: 생성자를 호출해서 객체를 생성.
연산자(new)와 생성자는 바늘과 실 같은 존재?


cat: 생성자 Constructor 

출처: https://nomad-programmer.tistory.com/152

---

궁감

null?

string?

cat?

void? public void?
---

class란?

객체를 정의해 놓은 것 or 객체를 생성하기 위한 설계도.

*객체?: 클래스에 정의된 내용이 메모리에 생성된 것.

인스턴스화: 클래스로부터 객체를 만드는 과정.

---

새 인스턴스 유형 만들기--> 왜 만드는데?



---

## 암시적 형식 지역 변수..Var..(implicitly typed local variable)

: 데이터 타입을 개발자가 아닌 컴파일러가 결정하게 만드는 키워드. 

할당된 오른쪽 값을 확인하여 컴파일러에 의해 왼쪽 변수 타입을 결정하게 된다. --> 컴파일러에게 변수의 타입을 명시적으로 알려주지 않아도 개발자를 대신하여 올바른 타입을 추론해줌.

※ 개발자가 올바른 반환타입을 알지 못해 올바르지 못한 타입을 명시적으로 지정하여 사용되는 경우를 방지한다.

but, 내장 숫자 타입(int,float,double..등등)은 다양하게 변화가 가능하다.(int<>double). 이들은 각각의 정밀도가 다르기 때문에 가독성과 정밀도에 있어서 오류가 발생할 수 있다.

---

참조: https://huiyu.tistory.com/entry/effective-C-%EC%A7%80%EC%97%AD%EB%B3%80%EC%88%98-%EC%84%A0%EC%96%B8%EC%9D%80-var%EB%A5%BC-%EC%82%AC%EC%9A%A9var-%EA%B8%B0%EC%B4%88


---

## 오름차순/ 내림차순

- 오름차순
Array.Sort(arrName);

- 내림차순

1. Array.Sort(arrName);
2. Array.Reverse(arrName);
--> 먼저 오름차순 정렬 후 뒤집기.

---

문자열 Sting

: 문자들의 집합.

문자 1개: char형 변수에 저장.

---

NULL 문자? ('\O')

이 문자의 끝을 알리기 위해 사용된다.

예) I like cat ---> 문자의 수: 8개 /실제 필요한 공간의 수: 9개
char형 배열에 문자를 저장하고 싶다면 반드시 문자의 개수+1에 해당하는 크기를 할당해 놓아야 한다.

cat의 t가 마지막 글자라는 것은 나만 알뿐이고 코드는 알 수가 없다.

---

## 관계연산자

: 두 개의 피 연산자의 값을 비교하여 그 결과를 참 or 거짓으로 나타내는 연산자.

두 연산자의 값이 같다: ==
두 연산자의 값이 다르다: !=
크거나 작다: >,<
크거나 같다, 작거나 같다: >=,<=

---

## 논리 연산자

: 주어진 논리식을 판단하여, 참, 거짓 판별.

&&: 
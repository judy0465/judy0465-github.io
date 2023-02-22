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

- ## 소수점 나눗셈 (반올림)

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








---








---








---
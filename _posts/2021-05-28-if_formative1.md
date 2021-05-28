---
layout: single
title: "조건문"
toc: true
toc_sticky: true
toc_label: "페이지 주요 목차"
---

### 01. 보안 카드 접수증  
![securitycard](/assets/images/securitycard_c.png)
~~~c
#include <stdio.h>
main()
{
 char name[4];
 int age;
 char code;
 float secure;
 printf("이름을 입력하세요: ");
 scanf("%s", &name);
 printf("나이를 입력하세요: ");
 scanf("%d", &age);
 fflush(stdin);
 printf("부서코드를 입력하세요: ");
 scanf(" %c", &code);
 printf("보안키를 입력하세요: ");
 scanf(" %f", &secure);
 printf("*********************\n");
 printf("이름: %s\n", name);
 printf("나이: %d\n", age);
 printf("부서코드: %c\n", code);
 printf("보안키: %.3f\n", secure);
 printf("*********************\n");
}
~~~

### 02. 성적 계산  
![scorecalculation](/assets/images/scorecalculation.png)
~~~c
#include <stdio.h>
 
int main()
{
 double a, b, c;
 int d, e, f;
 double score;
 printf("***과목별 점수 계산 프로그램 ***\n");
 printf("중간고사 반영비율/받은 점수를 입력하세요 : ");
 scanf("%lf %d", &a, &d);
 printf("기말고사 반영비율/받은 점수를 입력하세요 : ");
 scanf("%lf %d", &b, &e);
 printf("수행평가 반영비율/받은 점수를 입력하세요 : ");
 scanf("%lf %d", &c, &f);
 score = a*d + b*e + c*f;
 printf("점수는 %.1lf 입니다\n", score);
}
~~~

### 03. 사주보기  
![birthdateluck](/assets/images/birthdateluck.png)
~~~c
#include <stdio.h>
main()
{
 int year, month, day, res;
 printf("당신의 사주를 봐드립니다.\n연도, 월, 일을 차례대로 입력하세요 :");
 scanf("%d %d %d", &year, &month, &day);
 res=(year-month+day)%10;
 if(res==0)
   printf("당신의 사주는 대박입니다.\n");
 else
   printf("당신의 사주는 그럭저럭입니다.\n");
}
~~~

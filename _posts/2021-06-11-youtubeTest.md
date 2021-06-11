---
layout: single
title: "비트 연산자 (유튜브 동영상 삽입하기)"
categories: "개념 정리"
toc: true
toc_sticky: true
toc_label: "페이지 주요 목차"
---

{% include video id="Np8Eg9qj_YU" provider="youtube" %}


### 01. 사주보기
~~~c
#include <stdio.h>
int main(void)
{ int year,month,day,result;
printf("당신의 사주를 봐드립니다.\n");
printf("연도 월 일을 차례대로 입력하세요 : ");
scanf("%d,%d,%d",&year,&month,&day);
result=(year-month+day)%10;
if(result==0)
printf("당신의 사주는 대박입니다.\n");
else
printf("당신의 사주는 그럭저럭입니다.\n");
return 0;
}
~~~

### (1) 산술 연산자
~~~c
#include <stdio.h>
int main()
{
int a=10, b=3;
printf("a+b=%d\n", a+b);
printf("a-b=%d\n", a-b);
printf("a*b=%d\n", a*b);
printf("a/b=%d\n", a/b);
printf("a%%b=%d\n", a%b);
printf("-b=%d\n", -b);
return 0;
}
~~~

### (2) 관계 연산자
~~~c
#include <stdio.h>
int main()
{
int a=33, b=7;
printf("a>b -> %d\n", a>b);
printf("a<b -> %d\n", a<b);
printf("a>=b -> %d\n", a>=b);
printf("a<=b -> %d\n", a<=b);
printf("a==b -> %d\n", a==b);
printf("a!=b -> %d\n", a!=b);
return 0;
}
~~~

### (3) 증감 연산자
~~~c
#include <stdio.h>
int main()
{
int a=10;
printf("a++=%d\n", a++); //10 a=a+1
printf("++a=%d\n", ++a); //12
printf("a--=%d\n", a--); //12
printf("--a=%d\n", --a); //10
return 0;
}
~~~

### (4) 비트 연산자
~~~c
#include <stdio.h>
int main()
{
int x = 9;
int y = 10;
int z = 4;
printf("비트 AND = %08x\n", x & y);
printf("비트 OR = %08x\n", x | y);
printf("비트 XOR = %08x\n", x ^ y);
printf("비트 NOT = %08x\n", ~x);
printf("비트 << = %08x\n\n", x << 1);
printf("비트 >> = %08x\n", x >> 1);
return 0;
~~~

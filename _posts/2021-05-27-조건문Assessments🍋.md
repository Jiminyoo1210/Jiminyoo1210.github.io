---
layout: single
title: "조건문 Assessments🍋"
toc: true
toc_sticky: true
toc_label: 페이지 주요목차
categories: 수행평가
last_modified_at: 2021-06-17 T08:06:00-05:00
--- 

### 01. 사주보기
![saju](/assets/images/if1.jpg.PNG)
~~~c
#include <stdio.h>
main()
{
int a, b, c, res;
printf("당신의 사주를 봐드립니다.\n연도, 월, 일을 차례대로 입력하세요");
scanf("%d %d %d", &a, &b, &c );
res=a-b+c;
if(res%10==0)
  printf("당신의 사주는 대박입니다.\n");
else
  printf("당신의 사주는 그럭저럭입니다.\n");
  return 0;
}

~~~

### 02. 3개의 터널 통과
![tunnul](/assets/images/if2.jpg)
~~~c
#include <stdio.h>
main()
{
 int a, b, c;
 printf("세 터널의 높이를 차례대로 입력하세요:");
 scanf("%d %d %d", &a, &b, &c);
 if(a<=170)
   printf("충돌%d", a);
 else if(b<=170)
   printf("충돌%d", b);
 else if(c<=170)
   printf("충돌%d", c );
 else 
   printf("무사통과")
   return 0;
}
~~~

### 03. 이 달은 며칠까지 있을까?
![callenderl](/assets/images/if3.jpg.PNG)
~~~c
#include <stdio.h>
main()
{
 int a, b;
 printf("연도와 월을 입력하세요:");
 scanf("%d%d", &a, &b);
 printf("%d년 %d월의 마지막 날은", a, b);
 if(b==1||b==3||b==5||b==7||b==8||b==10||b==12)
   printf("31일");
 else if(b==4||b==6||b==9||b==11)
   printf("30일");
   else{
     if(a%4==0||a%100!=0||a%400==0)
       printf("29일");
     else
       printf("28일");
   }
   printf("입니다\n");
   return 0;
}
~~~

### 04. 30분 전
![time](/assets/images/예.png)
~~~c
#include <stdio.h>
main()
{int a, b;
 printf("연도와 월을 입력하세요:");
 scanf("%d%d", &a, &b);
 printf("%d년 %d월의 마지막 날은", a, b);
 if(b==1||b==3||b==5||b==7||b==8||b==10||b==12)
  printf("31일");
 else if(b==4||b==6||b==9||b==11)
   printf("30일");
 else{
  if(a%4==0||a%100!=0||a%400==0)
    printf("29일");
 else
 printf("28일");

   }
 printf("입니다\n");
   return 0;
}
~~~


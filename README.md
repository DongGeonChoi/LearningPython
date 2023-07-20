# LearningPython
0. 한글 주석: #-*-coding: utf-8 -*-
1.  대화형 프로그래밍 언어(인터프리터)
2.  변수는 snake_case
3.  연산자 우선순위 :
    3-1 : **
    3-2 : +X,-X,~X
    3-3 : *, @, /, //, %
    3-4 +,-
4. 자료형 : Integer(int), Floating Point(float)
           String(str), Boolaen(bool)
5. 문자열
   5-1 : "" or '' 사용 ,"" 내부에 '' 사용 가능, 여러줄은 "*3
   5-2 : 연결은 +변수+, 문자열의 경우 str(변수) 이용

6. 내장함수
   abs() : 절대값(abs(-5) == 5
   pow() : 제곱(pow(4,2)) == 4^2 == 16
   max() : 최대값(max(5,12)) == 12
   min() : 최소값(min(5,12)) == 5
   round() : (round(3.14 or 4.99)) == 3 or 5 #사사오입 법칙 따름

7. random
   from random import (random, uniform, randint , randrange, choice, sample, shuffle)
   random() : 0.0 ~ 1.0 <
   int(random() * 10) :  1 ~ 10 Integer
   randrange(1, 45) : 1 ~ 45 <

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
           String(str)_(immutable), Boolaen(bool)
5. 문자열
   - "" or '' 사용 ,"" 내부에 '' 사용 가능, 여러줄은 "*3
   - 연결은 +변수+, 문자열의 경우 str(변수) 이용
   

7. 내장함수
   abs() : 절대값(abs(-5) == 5
   pow() : 제곱(pow(4,2)) == 4^2 == 16
   max() : 최대값(max(5,12)) == 12
   min() : 최소값(min(5,12)) == 5
   round() : (round(3.14 or 4.99)) == 3 or 5 #사사오입 법칙 따름

8. random
   from random import (random, uniform, randint , randrange, choice, sample, shuffle)
   random() : 0.0 ~ 1.0 
   int(random() * 10) :  1 ~ 10 Integer
   randrange(1, 45) : 1 ~ 45 
   randint(4,28) : 4 ~ 28

9. 논리연산자
   - and
   - or
   - not
10. 비트연산자
    - & : 비트 논리곱
    - | : 비트 논리합
    - ^ : 비트 XOR, 둘이 다르면 1
    - ~ : 비트 논리부정
    - bin(정수) : 10진수 -> 2진수 변환
    - int(2진수, 2) : 2진수 -> 10진수 변환
    - <<: 비트이동
   
12. 슬라이싱
    변수[0:?] : 0~? 미만
    변수[-?:] : 뒤? 부터 끝

14. 반복문
    - for i in range(범위) :
    - while 조건(True or False) :
      
15. mutable & immutable Type
    - mutable : bytearray, list, set, dict
    - immutable : tuple, string, bytes, frozenset, int, float, complex, bool

16. 문자열 처리 함수
    - lower : 소문자
    - upper : 대문자
    - 변수[0].isupper() : 대문자 True?
    - len() : 길이
    - 변수.replace("기존 문자열", "대체 문자열") : 문자열 변경
    - 변수.index("문자열") : 몇번에 위치?,  "문자열", index + 1 그 뒤에
    - 변수.find("문자열") : 문자열 검색
    - 변수.count("문자열") : 몇번 등장 하는지
   

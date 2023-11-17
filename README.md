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
    - 변수.append("문자열") : 마지막에 문자열 삽임
      
17. 리스트
    - 변수 = [val, val, val]
    - 변수.insert(1,"문자열") : 1번 위치에 삽입
    - 변수.append("문자열") : 마지막에 문자열 삽임
    - 변수.pop("문자열") : 맨 뒤부터 꺼냄
    - 변수.sort() : 오름차순 정렬
    - 변수.reverse() : 순서 뒤집기
    - 변수.clear : 지우기
    - 변수 = ["asd",10,True] : 다양한 자료형 함께 사용 가능함 
    - 변수1 = extend(변수2) : 리스트 합침
   
18. 딕셔너리
    - 변수{key1 : value, key2 : value}
    - print(변수[key1]) : 대괄호가 들어가야 됨 (없는 값 출력 시 종료)
    - print(변수.get(key1)) : 위와 동일한 출력 (없는 값 출력 시 None 출력)
    - print(변수.get(key1, "사용 가능")) : None이 아닌 사용 가능 출력
    - print(key1 in 변수) : True, print(key3 in 변수) : False
    - 변수["key3"] = "value" : 삽입 및 업데이트 가능
    - del 변수["key"] : 삭제
    - print(변수.keys()) : 키만 출력
    - 변수.values() : value만 출력
    - 변수.items() : 쌍으로 출력
    - .clear : 지우기
   
19. if __name__ =='__main__':
    - 최초로 시작한 스크립트 파일과 모듈의 차이가 없기 때문에 어떤 스크립트 파일이던 시작점도 될 수 있고, 모듈도 될 수 있다. 그래서 name 변수를 통해 현재 스클비트 파일이 시작점인지 모듈인지 판단한다.
    - __name__은 python 내장함수로써 스크립트 파일의 이름(문자열)을 변수의 값으로 지정 됨
      (ex: donggeon.py == print(__name__) # donggeon
    - 그 **파일 안에서** 실행 해당 함수를 실행시키면 __name__ 변수에 담기는 것은 모듈의 이름이 아니라 __main__으로 값이 저장됨
    - 새로운 파일에서 import로 불러온 스크립트의 __name__ 변수에는 그 모듈이 담겨져 있음

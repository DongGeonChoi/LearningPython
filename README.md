# LearningPython
0. 한글 주석: #-*-coding: utf-8 -*-
1.  대화형 프로그래밍 언어(인터프리터)
2.  변수는 snake_case
3.  연산자 우선순위:
    3-1: **
    3-2: +X,-X,~X
    3-3: *, @, /, //, %
    3-4 +,-
4. 자료형: Integer(int), Floating Point(float)
           String(str)_(immutable), Boolaen(bool)
5. 문자열
   - "" or '' 사용 ,"" 내부에 '' 사용 가능, 여러줄은 "*3
   - 연결은 +변수+, 문자열의 경우 str(변수) 이용
   - 
   - a.upper() = a는 변수 .upper는 메소드 ()는 메소드를 실행하라는 의미를 가진다.
     괄호 안에는 메소드가 필요로하는 매개변수를 포함할 수 있음
 
   

7. 내장함수
   abs(): 절대값(abs(-5) == 5
   pow(): 제곱(pow(4,2)) == 4^2 == 16
   max(): 최대값(max(5,12)) == 12
   min(): 최소값(min(5,12)) == 5
   round(): (round(3.14 or 4.99)) == 3 or 5 #사사오입 법칙 따름

8. random
   from random import (random, uniform, randint , randrange, choice, sample, shuffle)
   random(): 0.0 ~ 1.0 
   int(random() * 10):  1 ~ 10 Integer
   randrange(1, 45): 1 ~ 45 
   randint(4,28): 4 ~ 28

9. 논리연산자
   - and
   - or
   - not
10. 비트연산자
    - &: 비트 논리곱
    - |: 비트 논리합
    - ^: 비트 XOR, 둘이 다르면 1
    - ~: 비트 논리부정
    - bin(정수): 10진수 -> 2진수 변환
    - int(2진수, 2): 2진수 -> 10진수 변환
    - <<: 비트이동
   
12. 슬라이싱
    변수[0:?]: 0~? 미만
    변수[-?:]: 뒤? 부터 끝

14. 반복문
    - for i in range(범위):
    - while 조건(True or False):
      
15. mutable & immutable Type
    - mutable: bytearray, list, set, dict
    - immutable: tuple, string, bytes, frozenset, int, float, complex, bool

16. 문자열 처리 함수
    - lower: 소문자
    - upper: 대문자
    - 변수[0].isupper(): 대문자 True?
    - len(): 길이
    - 변수.replace("기존 문자열", "대체 문자열"): 문자열 변경
    - 변수.index("문자열"): 몇번에 위치?,  "문자열", index + 1 그 뒤에
    - 변수.find("문자열"): 문자열 검색
    - 변수.count("문자열"): 몇번 등장 하는지
    - 변수.append("문자열"): 마지막에 문자열 삽임
    - join: 문자열 사이에 변수 값을 삽입한다. 리스트를 문자열로 만들때 사용한다.
      a = [a,b,c,d] "".join(a): abcd 
      
17. 리스트
    - 변수 = [val, val, val]
    - 변수.insert(1,"문자열"): 1번 위치에 삽입
    - 변수.append("문자열"): 마지막에 문자열 삽임
    - 변수.pop("문자열"): 맨 뒤부터 꺼냄
    - 변수.sort(): 오름차순 정렬
    - 변수.reverse(): 순서 뒤집기
    - 변수.clear: 지우기
    - 변수 = ["asd",10,True]: 다양한 자료형 함께 사용 가능함 
    - 변수1 = extend(변수2): 리스트 합침
   
18. 딕셔너리
    - 변수{key1: value, key2: value}
    - print(변수[key1]): 대괄호가 들어가야 됨 (없는 값 출력 시 종료)
    - print(변수.get(key1)): 위와 동일한 출력 (없는 값 출력 시 None 출력)
    - print(변수.get(key1, "사용 가능")): None이 아닌 사용 가능 출력
    - print(key1 in 변수): True, print(key3 in 변수): False
    - 변수["key3"] = "value": 삽입 및 업데이트 가능
    - del 변수["key"]: 삭제
    - 변수.keys: 키만 list형태로 출력 (dict_keys(['apple', 'banana', 'cat']))
    - keys로 출력 시 제약사항이 생기는데 .pop .insert .del 사용 불가
    - 변수.values(): value만 출력
    - 변수.items(): 쌍으로 출력
    - .clear: 지우기
   
19. if __name__ =='__main__':
    - 최초로 시작한 스크립트 파일과 모듈의 차이가 없기 때문에 어떤 스크립트 파일이던 시작점도 될 수 있고, 모듈도 될 수 있다. 그래서 name 변수를 통해 현재 스클비트 파일이 시작점인지 모듈인지 판단한다.
    - __name__은 python 내장함수로써 스크립트 파일의 이름(문자열)을 변수의 값으로 지정 됨
      (ex: donggeon.py == print(__name__) # donggeon
    - 그 **파일 안에서** 실행 해당 함수를 실행시키면 __name__ 변수에 담기는 것은 모듈의 이름이 아니라 __main__으로 값이 저장됨
    - 새로운 파일에서 import로 불러온 스크립트의 __name__ 변수에는 그 모듈이 담겨져 있음

20. 복소수
    - 1 + 2j의 절대값
    - 2.23607
    - 복소수의 실수 부분과 허수 부분을 각각 제곱한 후 더하고 그 합의 제곱근을 구해야 함
    - 실수는 일반적으로 우리가 일상적으로 사용하는 숫자
    - 허수는 실수로는 표현할 수 없는 숫자 (실수는 어떤 수의 제곱근도 음수가 될 수 없음 그렇기에 허수 단위 i 도입)
    - 1,2 각각 제곱한 후 더하고 그 합의 제곱근을 구해야 함 루트(1*1 + 2*2 = 1+4 = 루트5) 루트5의 제곱근이 절대값

21. 함수
    - def sum(함수명)(매개변수1, 매개변수2):
          변수 = 매개변수1 + 매개변수2 
          return 변수 **OR** return 매개변수1 + 매개변수2 
      prunt(sum(5,6))
    - 입력에 대한 결과를 만들어주는 역할을 하고, 반복입력 대체, 가독성 증가
    - 출력에 해당하는 값은 return 이후에 있는 내용을 출력해준다
    - 입력값의 개수를 정확하게 알지 못할 경우 변수 앞에 *를 추가하여 사용
    - 개수가 정해지지 않은 다수의 인자가 전달되면 모두 묶어서 한 개의 튜플 자료형으로 받음
    - 여러개의 출력값을 함께 출력해줄 수 있으며, 이 경우 튜플 형태로 출력
    - return 자체는 값을 반환 및 탈출 기능으로 사용 가능
    - 함수 매개변수의 기본값을 a = True 같은 향태로 지정 가능(기본값이 없는 변수와 공존할 경우 가장 뒤에 와야 됨)
    - def test(a,b,c = True):
      
22. 클래스
    - 객체 지향 언어의 특징으로 물체를 정의하고 해당하는 동작을 정의
    - 인스턴스트는 클래스를 통해 생성된 객체를 의미하고, 매소드는 클래스 내부에 정의된 **함수**를 의미한다.
    - 메소드는 필수적으로 입력을 self로 받아야만 한다
      class Test_Class:
          #생성자 메서드
          def __init__(self):
              self.result = 0
          def adder(self, num):
              self.result += num
              return self.result
    - 생성자는 class를 통해 인스턴스가 생성될 때 자동으로 동작하고
      class 내부에서 사용되는 변수를 초기화, 정의 하는 역할을 한다. 생성자가 없으면 class에 매개변수를 전달할 수 없음
    - 클래스로부터 만들어진 개체는 인스턴스라고 함

    class car:
        def __init__(self, brand, model):
            self.brand = brand
            self.model = model

        def display_info(self):
            print(f"This car is a {self.brand} {self.model}")

    #car 클래스로부터 인스턴스 생성 my_car, your_car라는 두 개의 인스턴스 생성
    my_car = car("Kia", "K5") 
    your_car = car("Hyndai", "Avante")
    #인스턴스 변수 접근
    print(my_car.brand)
    print(my_car.model)
    #메서드 호출
    my_car.display_info()
    your_car.display_info()

23. 클래스 상속
    - 부모의 기능을 그대로 받아올 수 있으며, 추가적으로 기능을 정의하여 사용할 수 있음
    - Method overriding이란 상속 받은 객체에서 동일한 이름으로 다른 역할을 하는
      메소드를 생성하는 것을 의미하며 이 경우 부모에 있는 메소드보다 자식에 있는 메소드가 우선적으로 동작
    - Method overriding 예시
    class Country:
        name = '국가명'
        population = '인구'
        captial = '수도'

        def show(self):
            print("국가 클래스의 메소드 입니다.")

        def show_name(self):
            print("국가의 이름을 알려줍니다.")

    class korea(Country):

        def __init__(self, name):
            self.name = name

        def show_name(self):
            print(f"국가의 이름은: {self.name}")

    - 
        
    

# JAVA-STUDY
자바 공부

어느정도 프로그래밍을 이해할 수 있게 된 지금, 다시 자바를 다뤄보자..
자바14 버전 사용.


------------------------------------------

    학습목표
     1. 기본개념
     2. 언어는 언어일 뿐 
     3. 이 책에서 1장~5장 / 6장~9장 / 11장 / 12장 / 15장 주력으로


<hr>

1. 자바를 시작하기 전에
   1. 자바란?
      1. OOP 언어
      2. 운영체제와 독립적
      3. 자바로 작성된 애플리케이션은 모두 가상컴퓨터(JVM)에서만 실행된다.
      4. api문서: http://java.sum.com/
      5. 실행과정
         1. *.class 파일 로드
         2. 파일 검사
         3. class에서 main호출
2. 변수
   1. 기본형 변수
      1. String은 char에 기능을 더한 것이다.
   2. 참조형 변수
   3. 형변환
      1. 표현번위가 좁은 쪽에서 넓은 쪽으로 형변환
3. 연산자
   1. 비트 연산자
      1. |(OR연산자)
      2. &(AND연산자)
      3. ^(XOR연산자)
   2. 삼항 연산자
      1. 조건식 ? 식1(참)0 : 식2(거짓)
4. 조건문과 반복문
   1. 조건문
      1. if
         1. 괄호 안이 참이되면 실행하라
         2. 블럭 내의 문장이 하나 뿐일 때는 ``{}``를 생략할 수 있다.
      2. switch
         1. 조건식 결과는 정수 또는 문자열이어야 한다.
         2. switch의 중첩도 가능
   2. 반복문
5. 배열
6. OOP1
   1. 장점
      1. 코드의 재사용성이 높다
      2. 코드관리가 용이
      3. 신뢰성이 높은 프로그래밍
   2. 변수의 종류
      1. 클래스 변수
         1. static
      2. 인스턴스 변수
      3. 지역 변수
   3. JVM의 메모리 구조
      1. Method Area
         1. JVM은 ``*.class``을 읽고 분석하여 이 영역에 저장한다.
      2. Heap
         1. 프로그램 실행 중 생성되는 인스턴스는 모두 이곳에 생성된다
      3. Call stack
         1. 메서드의 작업에 필요한 메모리 공간을 제공하며, 작업을 마치면 할당되었던 메모리 공간은 반환되어 비어진다.
   4. 객체를 생성하지 않고도 메서드를 호출할 수 있으려면, 메서드 앞에 ``static``을 붙여야 한다.
   5. 자바에서는 메서드를 호출할 때 복사호출한다.(그렇기 때문에 콜하는 structure의 값을 바꾸고 싶으면 참조형 매개변수를 변경해야 한다.)
      1. 기본형 타입
         1. 값이 복사
            1. read only
      2. 참조형 복사
         1. 인스턴스의 주소가 복사
            1. read & write
      3. 간단한 structure은 배열로 정의할 수 있다.(배열도 참조변수이므로)
   6. ``return``값이 있는 함수를 ``return``이 없어도 함수가 실행될 수 있게 가능(코드참조:``returnTest.java``)
   7. 참조형 반환타입(코드참조: ``ReferenceReturnEx.java``)
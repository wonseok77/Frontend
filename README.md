# Frontend
JSP는 쓰레드 단위다 because 프로세스 단위가 과부하가 걸리면 너무 느려서

##### JSP 특)
강력한 이식성  
서버 자원의 효율적인 사용
간편한 MVC(Model : business's logic , View :화면 html, Controller : 요청과 model 과 View를  매칭시켜주는 역할) 패턴 적용
JSTL, 커스텀태그 등을 이용한 개발 용이성  
  
MVC는 유지보수가 편하다 : 개발비용만큼 많이 드는게 유지보수 비용이기 때문에 장점임  
얼마나 유지보수가 편하냐에 따라서 Software 수명이 늘어난다

##### Servlet의 개요  
웹 서버상에서 실행되는 자바의 클래스 파일
javax.servlet.Servlet 인터페이스를 구현(Implements)해서 작성
입력과 출력을 HTTP 프로토콜 요청(Request)과 응답(Response)의 형태로 다룬다

##### get POST 방식
데이터를 요청하는 방법
사용자가 backend에 데이터를 올리는 방식  
  
get방식 : header에 올린다 (URL에 노출된다, 데이터의 크기가 정해져(256 바이트) 있어서 큰 데이터 불가)  
Post방식 :  body에 올린다 (body에 숨겨서 올려서 가시적이지 않다 : 회원가입 같은거, 중요한 데이터, 큰 데이터)

##### 웹 컨테이너(톰캣)
컨테이너에서 request response 생성 후 web.xml을 참조하여 해당 서블릿의 스레드 생성 후 service 메소드 호출  
  
service 메소드에서는 요청 방식에 따라 doGet이나 doPost 메소드 호출  
  
doGet이나 doPost 메소드에서 응답 생성  

##### JavaScriptPage
Context root

web.xml에서 불러오는 방법 시험

##### 주석(시험나옴)
HTML 주석  
JSP 주석  
<%-- JSP 주석입니다. %-->
자바 선언 변수? 코드 스크립틀릿?
JAVA스타일 주석  
<%! .... %> 여기 안에서 선언된 변수와 메서드의 정의만 들어간다 JSP로 변환된다.  

JSP 지시어(import를 할때도 쓴다, page 지시어 속성(language,extends,import,session,buffer,autoFlush ---등), include 지시어,    

<%@ ... %> 여기서 정의된거는 지역변수로 들어간다 Servlet으로 변환될때 서비스 메서드 안에, 골뱅이는 지시어 ?  

<%= %> 표현식 자바 함수의 결과값을 browser 화면에 출력할때 쓴다  

나중에는 EL 표기법으로 간단해지지만 알아두긴 해야한다

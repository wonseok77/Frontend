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
get header에 올린다 (URL에 노출된다, 데이터의 크기가 정해져있어서 큰 데이터 불가, )
Post방식은 body에 올린다 (body에 숨겨서 올려서 가시적이지 않다 : 회원가입 같은거, 중요한 데이터, 큰 데이터)




# SpringBoot-03
김영한 스프링 / 개인적인 공부

### View 환경설정
- spring boot 에서는 필요한 것을 찾는 능력이 중요합니다.
- 여기서 index.html을 만드는 것으로 예시를 들자면..
  - spring.io 접속
  - spring boot 접속
  - 맞는 버전에 대한 reference를 들어감
  - spring feature로 들어가서 find: welcome page [index.html] 찾아보기
    - spring boot는 먼저 index.html을 찾는다. static에 있는 index.html을 찾고 못찾으면 index template에서 찾아보고.. 이런 식 (공식 문서)
-  메뉴얼에서 검색을 할 수 있어야 합니다.

### thymleaf 템플릿 엔진

---
## 정적 컨텐츠
- 스프링부트는 기본적으로 제공함
- static folder 에 hello-static.html을 작성하고, web에서 접속 완료
  - 내장 톰켓 서버가 받고 스프링에 넘김
  - 스프링 컨테이너에 관련 컨트롤러가 없으니 static으로 감
    - 이건 컨트롤러에 우선권이 있다는 것임
  - 즉 resources에 있는 hello-static을 찾고 반환
## MVC (model - view - controller)와 템플릿 엔진
- 웹 브라우저에서 톰켓 서버로 주소를 보내면 스프링이 컨트롤러에서 찾아서 처리
- 스프링이 viewResolver(뷰를 찾아주고 엔진 연결)로 처리
- 랜더링 후 변환하여 웹브라우저에 반환을 해준다.
## API (Application Program Interface)
- @Responsebody : http에서 헤더와 바디로 나눌 때, 바디쪽의 데이터를 내가 직접 넣어주겠다.
- class를 생성해 getter/setter를 생성하고 진행
  - JSON (Key:Value의 구조) 형태로 데이터 반환됨
### Getter/Setter
---
# 실습?
- domain package
- repository
  - 회원 객체를 저장하는 저장소
  - Member interface


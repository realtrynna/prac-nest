# Slack Clone
https://docs.nestjs.com/

<br>

### 패키지
* npm i @nestjs/cli: 전역 명령어
* npm i @nestjs/config: 환경 변수 모듈

### CLI
https://docs.nestjs.com/cli/usages

* nest g mo user: UserModule
* nest g co user: UserController
* nest g s user: UserService 

<br>

### 특징 (추후 정리 예정)
0. Nest는 Module 기반임 __모듈로 패키징__ 한 라이브러리를 사용 
<br>

1. Nest는 Express 기반 (Express 기능은 Nest에서 사용 가능) 
<br>

2. Module을 직접 구현한다는 점에서 Spring보다 __IOC(Inversion Of Control)__ 가 약함 
<br>

3. 익스프레스는 Router 위주의 설계인 반면 네스트는 __Module__ 위주의 설계 
<br>

4. 비즈니스 로직을 __서비스__ 로 분리하는 이유는 __재사용__ 과 __테스트__ 를 위함 
<br>

5. __implements__ 는 에디터와 타입스크립트의 활용을 극대화하기 위함 
<br>

6. Service를 모듈 providers에 등록하면 내부적으로 DI 해줌 
<br>

7. req.body: @Req, req.query: @Query, req.params: @Param
<br>

8. Nest의 Dto 타입 Convention은 클래스
> 인터페이스는 타입스크립트 문법이므로 컴파일 후 제거됨 <br>
> 클래스는 자바스크립트 문법이라 런타임 단계에서 존재 <br>
> 클래스가 인터페이스 대체 가능
<br>

9. Controller ㅡ> Service ㅡ> Repository(TypeORM === Entity)
<br>

10. 
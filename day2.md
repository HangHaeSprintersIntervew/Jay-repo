1. spring sercurity란?
애플리케이션의 보안(인증과 권한, 인가 등)을 담당하는 스프링 하위 프레임워크

2. 브라우저에서 서버 응답까지의 흐름을 아는대로 설명
웹브라우저HTTP 메세지 생성 -> TCP/IP계층 전달 -> 패킷생성 -> (서버)패킷내부 HTTP메서드 분석해서 정보에 맞는 동작 -> (서버)HTTP응답 메시지 생성 -> (클라이언트)응답메시지 받아 동작

3. 객체지향관점에서 스프링 프레임워크를 바라봤을 때 장단점이 무엇인지
- 유지보수 및 기능의 확장성에서 용이함
- DI로 인한 느슨한 결합
-> 객체간 의존관계를 spring이 알아서 연관성을 맺어주기때문 
- AOP로 반복적인 코드제거 및 에러핸들링의 편의성

4. JWT에 대해서 간략히 설명
- 인증에 필요한 정보를 TOKEN에 담아 암호화 시켜 사용하는 방식을 의미
- JWT는 Header, Payload, Signature의 3 부분으로 이루어지며, Json 형태인 각 부분은 Base64Url로 인코딩 되어 표현
- header : 토큰 타입 및 해시 암호화 알고리즘
- payload : 토큰에 담을 정보, 정보의 한 조각을 claim이라 한다.
- signature : header base64 + payload base64 + SECRET_KEY

5. OAuth에 대해서 간략히 설명
- OAuth는 제3자 인증방식 입니다.신뢰할 수 있는 서버에게 정보를 맡겨놓고 접근할 수 있는 권한을 주는 것

6. 오버라이딩과 오버로딩이 무엇이고, 어떤 차이가 있는지 설명
오버라이딩 - 상위 클래스의 메서드를 하위클래스에서 재정의해서 사용하는것
오버로딩 - 같은 이름의 메서드를 가져야 할때 사용하는데 (생성자 오버로딩, 메서드 오버로딩) 파라미터의 유형과 갯수를 달리해서 다양한 호출에 응답.

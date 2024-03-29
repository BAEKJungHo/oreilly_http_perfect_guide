# 보안 HTTP

## HTTPS

https를 사용할 때, 모든 http 요청과 응답 데이터는 네트워크로 보내지기 전에 암호화된다.

https는 http 프로토콜에 대칭, 비대칭 인증서 기반 암호 기법의 강력한 집합을 결합한 것이다. https는 인터넷 애플리케이션의 성장을 가속한 동시에
웹 기반 전자상거래의 고속 성장을 이끄는 주력이다. https는 또한 분산된 웹 애플리케이션의 광역 보안 관리에 있어 대단히 중요하다.

https의 스킴 기본 포트는 443이다. 

## SSL 핸드셰이크

암호화된 HTTP 메시지를 보낼 수 있게 되기 전에, 클라이언트와 서버는 SSL 핸드셰이크를 할 필요가 있다.

핸드셰이크에서는 다음과 같은 일이 일어난다.

- 프로토콜 버전 번호 교환
- 양쪽이 알고 있는 암호 선택
- 양쪽의 신원을 인증
- 채널을 암호화하기 위한 임시 세션 키 생성

SSL은 서버 인증서를 클라이언트로 나르고 다시 클라이언트 인증서를 서버로 날라주는 상호 인증을 지원한다. 

## 오픈소스 라이브러리

몇 가지 SSL 클라이언트와 서버 프로그래밍을 쉽게 만들어주는 사용 혹은 오픈 소스 라이브러리들이 존재한다.

### OpenSSL

OpenSSL은 SSL과 TLS의 가장 인기 있는 오픈 소스 구현이다.

# 인터넷 대 웹(The Internet Versus the Web)

## 인터넷(The Internet)
- 인터넷은 수십억 대의 컴퓨터, 스마트폰 및 기타 장치를 전 세계적으로 연결하는 거대한 네트워크 인프라이다.
- 이 네트워크에서 연결된 모든 컴퓨터는 다른 연결된 컴퓨터와 통신할 수 있다.
- 인터넷을 통해 이동하는 데이터는 다양한 프로토콜을 통해 전송된다.


## 월드 와이드 웹(The World Wide Web)
- WWW 또는 간단히 웹이라고도 불린다.
- 인터넷을 통해 데이터에 접근하는 방법이다.
- 웹은 인터넷 위에 구축된 데이터 공유 모델이다.
- HTTP 프로토콜을 활용한다.


## 웹과 인터넷의 관계
- 웹은 인터넷의 일부분일 뿐이다.
- 이메일(SMTP 기반), FTP, 인스턴트 메시징 등은 인터넷의 일부이지만 웹의 일부는 아니다.
- **중요 포인트**: 웹은 인터넷의 하위 집합으로, 네트워크 컴퓨터를 통해 정보를 전송할 수 있는 많은 방법 중 하나이다.


---

# 클라이언트/서버 관계(Client/Server Relationship)

## 클라이언트(Clients)
- 클라이언트는 서버에 문서를 요청하는 소프트웨어이다.
- 사람들은 데스크톱 브라우저, 모바일 브라우저 및 기타 기술을 클라이언트로 사용하여 웹에서 문서에 접근한다.
- 개인용 기기(노트북, 스마트폰 등)가 클라이언트 역할을 한다.


## 서버(Servers)
- 요청에 따라 문서를 "제공하는" 컴퓨터는 서버라고 불린다. 보다 정확하게는 서버는 컴퓨터 자체가 아닌 소프트웨어이다.
- 서버 소프트웨어의 역할은 정보 요청을 기다린 다음, 해당 정보를 검색하여 가능한 빠르게 다시 보내는 것이다.
- 서버는 항상 네트워크에 연결되어 있다.


---

# 웹 페이지 주소(URLs)

## URL의 개념
- 웹의 모든 페이지와 리소스는 URL(Uniform Resource Locator)이라는 고유한 주소를 가진다.
- URL은 인터넷 상의 특정 자원의 위치를 나타낸다.


## URL의 구조
URL은 세 가지 주요 부분으로 구성된다:

1. **프로토콜(Protocol)**: 연결 방법을 정의
   - `http://`: URL이 정의하는 첫 번째 요소는 특정 트랜잭션에 사용될 프로토콜이다. HTTP는 서버에게 하이퍼텍스트 전송 프로토콜(Hypertext Transfer Protocol)을 사용하라고 알려준다.

2. **호스트명(Hostname) 또는 도메인**: 연결하려는 대상 식별
   - `www.exampleurl.com`: URL의 다음 부분은 도메인 이름으로 웹사이트를 식별한다. "www"는 서브도메인 이름이다. 이는 관습이 되었지만 필수는 아니다. 하나의 도메인에 여러 웹사이트(서브도메인)가 존재할 수 있다.

3. **경로(Path)**: 필요한 특정 파일 지정
   - `/info/aboutus.html`: 이는 서버의 디렉토리를 통한 요청된 HTML 문서까지의 절대 경로이다. 슬래시로 구분된 단어들은 루트 디렉토리(초기 /로 표시)부터 시작하는 디렉토리 이름이다.


## 문서 지정
- URL은 특정 문서를 지정할 수 있다: `http://www.explainthatstuff.com/howcomputerswork.html`
- 문서가 지정되지 않은 경우, 기본 문서가 반환된다.
- 기본 문서는 일반적으로 `index.html`이다.


## 최상위 도메인(Top-level domains)

### 원래 도메인
- .org
- .net
- .edu
- .gov
- .arpa


### 국가 도메인
- .au (호주)
- .br (브라질)
- .kr (한국)
- .mx (멕시코)
- .us (미국)


### 일반 도메인
- .wiki
- .biz
- .community
- .jobs
- .travel


---

# 프로토콜(Protocols)

## 프로토콜의 개념
- 프로토콜은 컴퓨터와 같은 전자 장치 간에 데이터를 전송하기 위한 규칙 또는 절차의 집합이다.
- 컴퓨터가 정보를 교환하기 위해서는 정보가 어떻게 구조화되고 각 측이 어떻게 정보를 주고받을 것인지에 대한 사전 합의가 있어야 한다.


## 주요 인터넷 프로토콜
- **HTTP** – 하이퍼텍스트 전송 프로토콜(Hypertext Transfer Protocol)
- **HTTPS** – 보안 하이퍼텍스트 전송 프로토콜(Secure Hypertext Transfer Protocol)
- **FTP** – 파일 전송 프로토콜(File Transfer Protocol)
- **SMTP** – 이메일 전송 프로토콜(Email Transfer Protocol)


---

# HTTP 프로토콜

## HTTP의 개념
- 하이퍼텍스트 전송 프로토콜(HTTP)은 웹에서 정보를 교환하기 위한 통신 프로토콜이다.
- 인터넷에서 웹페이지와 파일을 보내고 받는 데 사용된다.
- 팀 버너스-리(Tim Berners-Lee)에 의해 개발되었다.
- HTTP는 Mac이나 PC의 브라우저와 같은 클라이언트가 웹 서버와 어떻게 통신하는지 규정하는 규약의 집합이다.


## 요청/응답 사이클(Request/Response Cycle)
- HTTP는 클라이언트와 서버 간의 요청-응답 프로토콜로 작동한다.
- 이것은 사용자의 컴퓨터(클라이언트)가 페이지를 요청하고 서버가 적절한 파일로 응답할 때 발생하는 과정이다.
- 기본 과정:
  1. 클라이언트(브라우저)가 서버에 HTTP 요청을 보낸다
  2. 서버는 요청을 처리한다
  3. 서버는 클라이언트에게 HTTP 응답을 보낸다
  4. 클라이언트(브라우저)는 응답을 처리하고 페이지를 렌더링한다


## HTTP 요청 메서드(HTTP Request Methods)
- HTTP 요청 메서드는 클라이언트가 서버에게 특정 동작을 수행하도록 요청하는 방법을 정의한다.
- 가장 일반적인 메서드는 다음과 같다:
  - **GET**: 리소스 검색을 요청한다. 데이터를 가져오기만 하는 용도로 사용된다.
  - **POST**: 서버에 데이터를 제출한다. 폼 제출이나 데이터 생성에 사용된다.
  - **PUT**: 지정된 URL에 리소스를 생성하거나 업데이트한다.
  - **DELETE**: 지정된 리소스를 삭제한다.
  - **HEAD**: GET과 동일하지만 응답 본문 없이 헤더만 반환한다.
  - **OPTIONS**: 대상 리소스에 대한 통신 옵션을 설명한다.


### GET 요청 예시
```GET / HTTP/1.1 Host: www.facebook.com ...```
- GET은 무언가를 검색하려는 메서드이다.
- `/`는 기본 페이지 또는 홈페이지를 나타낸다.
- `HTTP/1.1`은 사용하고자 하는 HTTP 버전을 나타낸다.
- `Host: www.facebook.com`은 서버가 관리하는 여러 웹사이트 중에서 반환할 특정 웹사이트를 지정한다.


## 서버 응답
```HTTP/1.1 200 OK Content-Type: text/html ...```
- HTTP 헤더와 콘텐츠로 구성된다.
- 200은 요청이 성공적으로 처리되었음을 나타내는 많은 HTTP 상태 코드 중 하나이다.


## HTTP 상태 코드(Status codes)
- **200 OK**: 요청 성공
- **301 Moved Permanently**: 영구 이동 (웹사이트가 현재 다른 주소에 있음)
- **302 Found**: 임시 이동 (일시적으로 이동됨, URL 리다이렉션을 수행하는 일반적인 방법)
- **304 Not Modified**: 수정되지 않음
- **401 Unauthorized**: 권한 없음
- **403 Forbidden**: 접근 금지 (특정 페이지에 접근 권한 없음)
- **404 Not Found**: 찾을 수 없음
- **500 Internal Server Error**: 서버 내부 오류 (웹 서버 자체의 코드에 오류가 있음)


---

# IP 주소(IP Address)

## IP 주소의 개념
- IP 주소는 인터넷에 연결된 각 장치를 식별하는 고유한 주소이다.
- 인터넷상의 모든 장치는 통신을 위해 IP 주소를 필요로 한다.


## IP 주소 버전

### IPv4
- 인터넷 프로토콜 버전 4(IPv4)는 32비트 주소를 사용한다.
- 약 43억 개(4,294,967,296 = 2^32)의 고유한 조합을 표현할 수 있다.
- 예: 192.168.1.1


### IPv6
- 인터넷 프로토콜 버전 6(IPv6)은 128비트 주소를 사용한다.
- 2^128개의 고유한 조합을 표현할 수 있다. (약 3.4 × 10^38개)
- 예: 2001:0db8:85a3:0000:0000:8a2e:0370:7334


## 사설 IP 주소(Private IP Addresses)
- 사설 IP 주소는 내부 네트워크에서만 사용되는 인터넷과 연결되지 않는 IP 주소이다.
- 사설 IP 주소는 라우터와 같은 네트워크 장치에서 네트워크 주소 변환(NAT)을 통해 제공된다.
- NAT의 주요 용도는 조직이나 기업이 사용해야 하는 공용 IP 주소의 수를 제한하여 경제성과 보안을 유지하는 것이다.


## DHCP(Dynamic Host Configuration Protocol)
- DHCP 서버는 네트워크의 각 장치에 IP 주소를 동적으로 할당하여 다른 IP 네트워크와 통신할 수 있게 한다.
- DHCP 서버는 IP 주소 풀을 유지하고 네트워크에서 시작할 때 DHCP 지원 클라이언트에게 주소를 임대한다.
- IP 주소가 정적(영구 할당)이 아닌 동적(임대)이기 때문에 사용되지 않는 주소는 자동으로 풀로 반환되어 재할당된다.


## DNS(Domain Name System)
- DNS(도메인 이름 시스템)는 네트워크 이름과 IP 주소의 디지털 데이터베이스를 포함하는 대규모 서버 네트워크이다.
- DNS는 사용자 친화적인 도메인 이름을 고유한 IP 주소에 할당하는 시스템이다.
- 예: 'www.example.com'이라는 도메인 이름을 '192.0.2.1'과 같은 IP 주소로 변환한다.
- 이를 통해 사용자는 복잡한 IP 주소 대신 기억하기 쉬운 도메인 이름을 사용할 수 있다.


## 내 IP 주소 확인하기
- Windows에서는 명령 프롬프트에서 `ipconfig` 명령을 통해 자신의 IP 주소를 확인할 수 있다.
- 또한 Windows 설정의 네트워크 속성에서도 IP 주소 정보를 확인할 수 있다.
- IPv4 주소(예: 192.168.1.116)는 로컬 네트워크에서 장치를 식별하는 데 사용된다.
- 공용 IP 주소와 사설 IP 주소는 일반적으로 다르며, 사설 IP 주소는 일반적으로 192.168.x.x와 같은 형식을 갖는다.


## 웹사이트의 IP 주소 찾기
- 명령 프롬프트에서 `nslookup` 명령을 사용하여 웹사이트의 IP 주소를 찾을 수 있다.
- 예: `nslookup google.com`은 구글 서버의 IPv4 및 IPv6 주소를 보여준다.
- 이 방법은 웹사이트가 어떤 IP 주소에 호스팅되어 있는지 확인하는 데 유용하다.


---

# 라우터(Routers)

## 라우터의 개념
- 라우터(게이트웨이)는 컴퓨터 네트워크 간에 데이터 패킷을 전달하는 네트워킹 장치이다.
- 라우터는 인터넷에서 트래픽 방향을 지정하는 기능을 수행한다.
- 데이터 패킷은 일반적으로 목적지에 도달할 때까지 네트워크를 통해 한 라우터에서 다른 라우터로 전달된다.
- 가정용 라우터와 데이터센터 라우터 등 다양한 종류가 있다.


## 라우팅 경로 추적
- 인터넷 프로토콜(IP) 네트워크를 통한 패킷의 경로를 표시하고 전송 지연을 측정하는 것이 가능하다.
- 이를 위해 `traceroute`(유닉스/리눅스) 또는 `tracert`(윈도우) 명령어를 사용할 수 있다.
- 이 명령어는 패킷이 목적지까지 가는 경로의 각 라우터 위치와 지연 시간을 보여준다.


---

# TCP/IP 프로토콜

## TCP(Transmission Control Protocol)의 개념
- 서버는 여러 유형의 요청에 응답할 수 있다.
- 서버가 웹페이지, 이미지, 이메일 등 어떤 종류의 요청을 받았는지 어떻게 알 수 있을까?
- TCP(전송 제어 프로토콜)는 보내는 "봉투의 외부"에 또 다른 번호를 추가하여 서버에서 원하는 서비스를 지정하는 표준이다.
- 이 번호는 특정 서비스에 해당하는 포트 번호이다.


## 표준 포트 번호와 프로토콜
- **22**: SSH (보안 셸)
- **53**: DNS (도메인 네임 시스템)
- **80**: HTTP (웹페이지)
- **443**: HTTPS (보안 웹페이지)
- **587**: SMTP (이메일 전송)


## 포트 번호 사용 예시
- `Google.com:80`은 구글의 웹서버에 HTTP 프로토콜을 사용하여 접속한다는 의미이다.
- 전화 통화 유추: IP 주소는 전화번호와 비슷하고, 포트 번호는 내선 번호와 유사하다.


## TCP/IP의 데이터 전송 방식
- 이미지나 비디오와 같은 대량의 데이터를 전송할 때, 데이터는 많은 작은 조각(패킷)으로 나뉜다.
- 이 조각들에는 순서 번호가 매겨져서 수신자가 모든 조각을 받았는지 확인할 수 있다.
- 일부 데이터 조각이 누락된 경우, 수신자는 서버에 해당 조각을 재전송하도록 요청할 수 있다.
- 이 방식은 데이터의 안정적인 전송을 보장한다.
# T82 Tickets

## 프로젝트 목표

## 진행 기간

2024-07-02 ~ 2024-08- 23

**결제 Service**  https://github.com/T82-encore/T82-payment.git

**쿠폰 Service** https://github.com/T82-encore/T82-Coupon.git

**좌석 Service** https://github.com/T82-encore/T82-Seat.git

**Push 알람 Service**  https://github.com/T82-encore/T82-Push.git

**회원 Service**  https://github.com/T82-encore/T82-User.git

**공연 Service** https://github.com/T82-encore/T82-Event.git

**댓글 Service** https://github.com/T82-encore/T82-Review.git

**티켓 Service**  https://github.com/T82-encore/T82-Ticket.git

**공통 예외 Service** https://github.com/T82-encore/T82-Common-Exception.git

**IOS Service** https://github.com/T82-encore/IOS_T82.git

## 기획 의도

이번 프로젝트의 주요 목표는 콘서트, 연극, 기타 문화 이벤트의 티켓 구매를 ‘조금 더 사용자 친화적이게 공연 예술을 지원하는 것이 어떨까?’ 라는 관점에서 출발 했습니다. **T82**는 많은 고객에게 다양한 문화 생활에 쉽게 접근할 수 있도록 하여 접근성을 높이며, 각 공연의 커뮤니티 참여를 촉진해 많은 사람들에게 문화 생활을 장려하기 위해 기획 되었습니다.

## 협업 관리

저희는 이번 협업 관리를 깃허브의 Project로 진행 하게 되었습니다.
![image (7)](https://github.com/user-attachments/assets/cf3ee942-df71-4a50-a7cc-8782646b34b2)

![image (8)](https://github.com/user-attachments/assets/bce5eeef-eaba-4443-ad05-1c3ae129569e)

![화면 캡처 2024-08-20 125224](https://github.com/user-attachments/assets/8303cff1-8123-482f-abae-d55c89064d1c)

**BackLog : 매 주 마다 개발 해야 할 기능의 목록들의 집합**

**Todo :  그 날 마다 해야 할 기능들의 집합**

**In Progress : 현재 (개발)진행중인 기능들의 집합**

**CodeReview : 개발이 완료되어 merge 되기를 기다리는 기능들의 집합**

**Done : CodeReview를 끝내고 merge 가 된 기능들의 집합**

**Cancled :  BackLog에는 있었지만 진행 도중 취소된 기능들의 집합**

 ****

## 디자인
![image (9)](https://github.com/user-attachments/assets/a09c8cbe-e8c6-47a8-a21d-1d65b0ea6fc4)


## ERD(1차 ~ 최종까지 변경사항)

[https://eastern-orchid-c48.notion.site/T82-Making-4f2615061845453fa3d7ca755da312b7?pvs=4](https://www.notion.so/4f2615061845453fa3d7ca755da312b7?pvs=21)


![image (10)](https://github.com/user-attachments/assets/1e76347a-05a1-45be-98e6-95925d6ab3f6)


이번 프로젝트는 MSA를 도입하게 되었는데 도입하게 된 이유는 아래와 같습니다.

### 도입 이유

### 1. 장애격리

티켓팅 플랫폼의 높은 트래픽에 대한 예상으로 개별 서비스로부터 장애가 옮겨가는 것을 막기 위해 결제 서비스에 문제가 생기더라도 이벤트 조회 등 다른 서비스들은 정상적으로 동작하는 것에 목적을 두어 서비스의 가용성을 높이기 위해 적용 했습니다

### 2. 확장성

MSA의 특징인 각 서비스가 독립적으로 배포되는 것을 이용하기 위해 티켓팅이라는 도메인의 특징인 인기 있는 티켓에 대한 티켓팅이 시작 될 때 이벤트에 관한 서비스만을 확장하여 자원 관리 부분에서 장점이 있을 것으로 생각되어 적용했습니다.

### 3. 트래픽 관리

티켓팅 도메인에서 이벤트 예약이 시작할 때 급증하는 트래픽에 관해서 MSA의 트래픽 분산을 통한 시스템 성능을 유지하는 것을 기대하여 적용하게 되었습니다.

## UserFlow

## System Architecture
**1차 System Architecture**
![T82 drawio (1)](https://github.com/user-attachments/assets/597ad735-acb7-4eb5-b9f8-45e743040608)

## 사용 기술

1. 프로그래밍 언어 및 프레임워크
- Spring boot 3
- Java 17
- Swift 5.1
- SwiftUI

2. 데이터 베이스
- MySQL
- Redis
- Firebase

3. 클라우드
- Google Cloud Platform
- AWS Lambda
- AWS S3
- AWS EKS
- AWS API GateWay

4. 컨테이너 및 오케스트레이션
- Docker
- Kubernetes

5. CI/CD
- Jenkins
- Xcode Cloud
- TestFlight

6. 메세지 브로커
- apache kafka

7. 부하 테스트 도구
- Jmeter

8. 라이브러리
- Feign
- GRPC
- jitpack
- Alamofire
- PopupView
- CoreMotion



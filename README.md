# PDGStudio 관리 웹앱(PWA) 서비스

<img width="1099" alt="image" src="https://github.com/user-attachments/assets/10c97c41-b083-4688-bfc6-dd50cc8bfcd6" />


## 왜 만들어졌을까요 ?


원래는 TimeBlock이라는 어플을 사용하려했습니다.
하지만 카테고리 설정이 너무 애매했고 색상도 잘 매치가 안됐어요
그리고 돌린이가 사용하기 힘들다고 했었고,
그녀는 작업실 회계관리를 위해 가계부 어플까지 따로 다운받아야했어요

그래서 제가 만들어보겠다 선언했습니다.

사실 가계부 어플 이야기 전엔 작업실 사용 일정관리뿐만 구상했지만,
돌린이의 요구사항으로는 우리의 월세 공과금 등 작업실 통장내역 관리도 있으면 좋겠다고 하여
금융관리까지 구현하게 되었어요.

최근에 타프로젝트에서 native 세팅을 하게 되면서 PWA라는 좋은 기술을 알게되어
이동중에도 관리가 편하게 되어야하잖아요 ?
그래서 사파리로(셋다 아이폰) 홈화면에 앱처럼 다운받을수있게 해야했어요
일정 등록시 푸쉬알림까지 와야하니깐 !


## 기술 스택 선정 !


1. 프론트엔드:
   
React
Material UI
React Router
Moment.js
React Big Calendar
LocalizationProvider (MUI X-date-pickers)

빠르게 개발을 해야해서 ts보단 js를 사용하게 되었어요.

2. 백엔드:

NestJS
TypeORM
PostgreSQL
JWT 인증

Java로 개발할수도 있었지만 이제는 Node.js로 백엔드 개발하는게 조금은 더 편해졌답니다.

3. 클라우드 & 배포:

Firebase Cloud Messaging (푸시 알림)
Vercel (프론트엔드 배포)
Railway (백엔드 배포)

이건 그렇게 크지도 않은 어플이고 트래픽도 높지않을테니 간편하게 배포할수있는 플랫폼을 선정했어요.

4. PWA 기능:

서비스 워커
매니페스트 파일
홈 화면 추가 기능
푸시 알림

제일 중요했던건 앱처럼 푸시알림을 위해 PWA 기능을 넣었습니다.


## 무슨 기능이 있을까요 ?

- 로그인

<img width="659" alt="image" src="https://github.com/user-attachments/assets/f7ca02e1-cbb2-446c-b3fe-562baeb37b1e" />

- 일정관리

<img width="984" alt="image" src="https://github.com/user-attachments/assets/4b09f505-5063-4579-9ba6-036c27194012" />
<img width="970" alt="image" src="https://github.com/user-attachments/assets/eb2eeb28-bb23-4f47-8667-061900cd3247" />
<img width="625" alt="image" src="https://github.com/user-attachments/assets/dff5cce3-6d4f-4c19-b7e5-76671f7a31e7" />

- 금융관리

<img width="774" alt="image" src="https://github.com/user-attachments/assets/66b07966-4c8e-484c-9f3b-c6adc603be3f" />
<img width="725" alt="image" src="https://github.com/user-attachments/assets/402fe14c-bbfb-472d-ac85-9452202299ba" />
<img width="965" alt="image" src="https://github.com/user-attachments/assets/242466bd-4230-406b-b0a1-54b8c50bc222" />


추후 더 예쁜 디자인을 할것이고, 금융관리 쪽은 좀 더 수정 할 예정입니다



 














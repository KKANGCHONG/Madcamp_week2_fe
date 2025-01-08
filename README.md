# 1. 개요
##  “What to do_ : 친구와 함께하는 일정 관리” ㅡ 프론트엔드 레포지토리
<img width="229" alt="app_icon" src="https://github.com/user-attachments/assets/bc4b687a-fda9-4265-994b-fbfaaa6d38fc" />

# 1.1. 프로젝트 소개

### 📗 BACKGROUND
요즘 대학생들은 점점 더 많은 할 일과 약속을 관리해야 하는 상황에 놓여 있습니다. 단순히 개인 일정 관리를 넘어, 친구들과 일정 공유 및 협력이 가능한 플랫폼이 필요합니다!

### 📗 GOAL
사용자 친화적인 UI를 통해 개인 일정과 할 일을 관리할 뿐만 아니라, 친구의 일정 확인, 시간표 공유를 활용한 일정 관리를 제공하는 앱을 개발하고자 했습니다.

---

# 1.2. Tech Stack

- **Front-End**: Flutter  
- **Back-End**: FastAPI  
- **Database**: SQLite  
- **IDE**: Android Studio, Visual Studio Code  
- **Version Control**: GitHub


# 2. 팀원 소개

| ![이명규]![myeongkyu](https://github.com/user-attachments/assets/c7c8a60f-c6ef-41bb-9055-d1ab42743ec5)| ![이현정]![hyunjung](https://github.com/user-attachments/assets/e4dd9a33-560a-4bc4-92bb-855deaaee15e)|
|---------------------------------|---------------------------------|
| **이명규**                      | **이현정**                      |
| - KAIST 전산학부 20학번         | - 이화여자대학교 컴퓨터공학과 22학번 |
| - [GitHub: mgklee](https://github.com/mgklee) | - [GitHub: KKANGCHONG](https://github.com/KKANGCHONG) |


# 3. API 명세서

| **Endpoint**                              | **Method** | **Description**               |
|-------------------------------------------|------------|-------------------------------|
| `/users/login`                            | POST       | 카카오 로그인 및 회원가입       |
| `/users/{user_id}/todos`                  | GET        | 사용자 할 일 목록 조회          |
| `/users/{user_id}/todos`                  | PUT        | 사용자 할 일 목록 업데이트      |
| `/users/{user_id}/friends/todos`          | GET        | 친구들의 할 일 목록 조회        |
| `/users/{user_id}/friends`                | GET        | 친구 목록 조회                 |
| `/friends`                                | POST       | QR 코드로 친구 추가            |
| `/users/{user_id}/timetable`              | POST       | 시간표 저장                   |
| `/users/{user_id}/timetable/{year}/{season}` | GET       | 시간표 조회                   |

# 4. ERD
![image](https://github.com/user-attachments/assets/27d2b19c-b43c-44a3-9adb-990e53513044)

# 5. 기능 소개
## 5.0. 로그인 화면
- 카카오 소셜 로그인 구현
## 5.1. To-do 리스트 탭

- 사용자가 할 일을 생성, 수정, 삭제 가능
- 상단에 주간 캘린더를 위치해 날짜별로 할 일 확인
- 공개 여부 설정 가능
## 5.2. 시간표탭

- 에브리타임 API를 연결해 URL를 입력하면 2차원 배열로 변환
- 변환된 배열을 통해 시간표 생성
- 친구들을 선택하면 해당 친구와 겹쳐진 시간표 확인 가능
## 5.3. 친구탭
- 개 여부가 오픈된 일정을 카테고리 별로 나눠 볼 수 있음
- 상단에 주간 캘린더가 위치해 날짜 별로 친구들의 할 일 확인 가능
## 5.4. 마이페이지
- QR 코드를 통해 손쉽게 친구 추가
- 친구 목록 확인 가능
- 이용 약관 확인 가능
- 로그아웃

## 6. 개발 후기
### 이명규
너무 빠르게 지나간 일주일이었습니다. 프론트엔드만 개발한 첫 주도 벅찼는데 백엔드까지 개발하라니 처음에는 막막했지만, 현정이와 나름 케미가 잘 맞아서 즐겁게 개발할 수 있었던 2주차였습니다. 놓고 싶은 기능도 많고 놓친 디테일도 많으니, 그래도 원래 계획했던 만큼은 이슈도 낸 것 같아 뿌듯합니다!

### 이현정
프론트엔드와 백엔드 레포를 나눠서 관리하거나 각각의 세부적인 기능 등, 처음 시도해볼게 많은 프로젝트였어요. 그리고 프론트 고마미 재부탁부터 백엔드 로직 작성, 서버 구성, 코든 구현 등 쉬운 작업은 없었지만, 맡겨준 백엔드 일을 하나씩 해결할 때마다 엄청 뿌듯했던 경험도 있었네요. 어렵지만 좋은 레벨업의 시간이었다고 생각하고 혼자서는 부족했던 디테일한 업무 부분까지 마무리할 수 있었어요! 특별히 많은 응원과 진행한 2주차 즐겁겠지? 맘속 감사를 전달합니다 👍
  

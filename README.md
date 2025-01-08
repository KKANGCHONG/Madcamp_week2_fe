# 1.1. 프로젝트 소개

### 🟩 BACKGROUND
요즘 대학생들은 점점 더 많은 할 일과 약속을 관리해야 하는 상황에 놓여 있습니다. 단순히 개인 일정 관리를 넘어, 친구들과 일정 공유 및 협력이 가능한 플랫폼이 필요합니다!

### 🟩 GOAL
사용자 친화적인 UI를 통해 개인 일정과 할 일을 관리할 뿐만 아니라, 친구의 일정 확인, 시간표 공유를 활용한 일정 관리를 제공하는 앱을 개발하고자 했습니다.

---

# 1.2. Tech Stack

- **Front-End**: Flutter  
- **Back-End**: FastAPI  
- **Database**: SQLite  
- **IDE**: Android Studio, Visual Studio Code  
- **Version Control**: GitHub


# 팀원 소개

| ![이명규]![myeongkyu](https://github.com/user-attachments/assets/c7c8a60f-c6ef-41bb-9055-d1ab42743ec5)| ![이현정]![hyunjung](https://github.com/user-attachments/assets/e4dd9a33-560a-4bc4-92bb-855deaaee15e)|
|---------------------------------|---------------------------------|
| **이명규**                      | **이현정**                      |
| - KAIST 전산학부 20학번         | - 이화여자대학교 컴퓨터공학과 22학번 |
| - [GitHub: mgklee](https://github.com/mgklee) | - [GitHub: KKANGCHONG](https://github.com/KKANGCHONG) |


# API 명세서

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

# ERD

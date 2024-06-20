![transparent](https://capsule-render.vercel.app/api?type=waving&color=3767a6&fontColor=fff&text=🛫GroupAir&height=250&fontSize=70&fontAlignY=40)

<br>

<h2 align="center" style="color:#96b3d9"> 그룹웨어 기본 연동 기능 및 메세지 봇 구현 </h2>

<br>

## 📕프로젝트 소개

- 항공에서 근무하는 직원이 출결 및 게시판 사용, 항공편 조회 등을위한 사이트
- 직원이 명확하게 이해하기 쉽고 부서 간 의사소통이원활하게 기능하는 조직도 구현
- 대표이사, 부장, 사원 권한에 따라 관여할 수 있는 부분 제한
- 한 눈에 알아볼 수 있는 UI 및 사용가치 있는 설계

| 작업파일                                                                                                 |
|------------------------------------------------------------------------------------------------------|
| [그룹웨어 기본 연동 기능 및 메세지 봇 구현](https://github.com/Jmgjava/team_project2/tree/master/Project2GroupAirTeam) |

<br>

## 💻사용프로그램

<span>
<img src="https://img.shields.io/badge/intellij IDEA-000000?style=flat&logo=intellij IDEA&logoColor=white"/> 
<img src="https://img.shields.io/badge/visualstudio-0075c6?style=flat&logo=visualstudio&logoColor=white"/> 
<img src="https://img.shields.io/badge/java-007396?style=flat&logo=java&logoColor=white"/> 
</span>
<br>
<span>
<img src="https://img.shields.io/badge/queryDsl-4479A1?style=flat&logo=queryDsl&logoColor=white"/>
<img src="https://img.shields.io/badge/gradle-02303A?style=flat&logo=gradle&logoColor=white"/>
<img src="https://img.shields.io/badge/mysql-4479A1?style=flat&logo=mysql&logoColor=white"/> 
</span>
<br>
<span>
<img src="https://img.shields.io/badge/springboot-6DB33F?style=flat&logo=springboot&logoColor=white"/>
<img src="https://img.shields.io/badge/spring data JPA-6DB33F?style=flat&logo=spring data JPA&logoColor=white"/> 
</span>
<br>
<span>
<img src="https://img.shields.io/badge/html5-E34F26?style=flat&logo=html5&logoColor=white"/>
<img src="https://img.shields.io/badge/css3-1572B6?style=flat&logo=css3&logoColor=white"/>
<img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=JavaScript&logoColor=white"/> 
</span>
<br>
<span>
<img src="https://img.shields.io/badge/kakaoMap-FFCD00?style=flat&logo=kakao&logoColor=white"/>
<img src="https://img.shields.io/badge/openweather-ea6e4b?style=flat&logo=openweather&logoColor=white"/>
</span>
<br>
<span>
<img src="https://img.shields.io/badge/thymeleaf-005F0F?style=flat&logo=thymeleaf&logoColor=white"/>
<img src="https://img.shields.io/badge/jquery-0769AD?style=flat&logo=jquery&logoColor=white"/>
</span>
<br>
<span>
<img src="https://img.shields.io/badge/komoran-000000?style=flat&logo=komoran&logoColor=white"/>
</span>
<br>

<br>


## 📁ERD
![img_6.png](/img/img_6.png)

<br>

## 🙍‍♂️팀원
| 이름  | 작업                                            |
|-----|-----------------------------------------------|
| 조민근 | layout(index), OpenWeather API, 부서관리, ChatBot |
| 서** | 회사일정, 게시판 관리                                  |
| 박** | 권한별 INDEX 페이지, 근태관리, 급여관리, 항공편관리(kakao map)   |
| 손** | cicd, db설계, 로그인, 사원관리 oauth, Mail, 조직연동       |
| 정** | 결재관리                                          |

<br>

## ✍작업내용

- [**layout**](#layout)
    - 공통으로 사용하는 header, menuBar 구현
- [**OpenWeather API**](#OpenWeather-API)
    - 날씨 정보 가져와 실시간 지역 날씨 정보 구현
- [**부서관리**](#부서관리)
    - 부서 생성, 조회, 수정, 삭제
- [**chatBot**](#chatBot)
    - 직원의 전화, 부서, 이메일 조회
    - 지역의 날씨 조회

<br>

### layout

- 공통으로 사용하는 부분 xmlns:layout 으로 구현

| layout 구현                                                                                                |
|----------------------------------------------------------------------------------------------------------|
| ![layout](https://github.com/Jmgjava/JMG_projects/assets/154856565/9c97de23-464b-45d4-9c07-a6874e09577f) |

### OpenWeather API

- openweather 에서 날씨 정보를 가져와 위치에 맞는 날씨 구현

| layout 부분 weather                                                                                         |
|-----------------------------------------------------------------------------------------------------------|
| ![weather](https://github.com/Jmgjava/JMG_projects/assets/154856565/8d66fefa-093e-477e-ba6b-61cbafb53a40) |

### 부서관리

- 부서 생성, 조회, 수정, 삭제

| 부서 생성                                                                                                          |
|----------------------------------------------------------------------------------------------------------------|
| ![department_C](https://github.com/Jmgjava/JMG_projects/assets/154856565/c6853801-7be1-4204-913a-476f2b6a581e) |

| 부서 조회,수정                                                                                                        |
|-----------------------------------------------------------------------------------------------------------------|
| ![department_RU](https://github.com/Jmgjava/JMG_projects/assets/154856565/f81ecf1a-4bd2-4621-80da-58daa1d7be0b) |

| 부서 삭제                                                                                                          |
|----------------------------------------------------------------------------------------------------------------|
| ![department_D](https://github.com/Jmgjava/JMG_projects/assets/154856565/de12d69e-e7b2-4cb4-b48f-bae577a8edd0) |

### chatBot

- 직원의 전화, 이메일, 부서 중 하나를 물어보면 그에 맞는 정보 텍스트로 전달

| 직원 검색                                                                                                            |
|------------------------------------------------------------------------------------------------------------------|
| ![chatBot_member](https://github.com/Jmgjava/JMG_projects/assets/154856565/8d90d86e-1c13-4f61-92c7-f80a90c62e8e) |


<br>

![transparent](https://capsule-render.vercel.app/api?type=soft&color=324153&fontColor=fff&text=감사합니다.&animation=fadeIn&height=100&fontSize=40&descAlignY=80&descAlign=70)
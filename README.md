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
| ![layout](https://github.com/Jmgjava/team_project2/assets/154856565/9bd4352c-5a22-4c9e-8550-beb1a25005cd) |

### OpenWeather API

- openweather 에서 날씨 정보를 가져와 위치에 맞는 날씨 구현

| layout 부분 weather                                                                                         |
|-----------------------------------------------------------------------------------------------------------|
| ![weather](https://github.com/Jmgjava/team_project2/assets/154856565/9d31e65f-a4bd-41ba-83c5-5084c39edec4) |

### 부서관리

- 부서 생성, 조회, 수정, 삭제

| 부서 생성                                                                                                          |
|----------------------------------------------------------------------------------------------------------------|
| ![department_C](https://github.com/Jmgjava/team_project2/assets/154856565/3d5b82a6-2a4b-42f1-9579-ee9fda771e1a) |

| 부서 조회,수정                                                                                                        |
|-----------------------------------------------------------------------------------------------------------------|
| ![department_RU](https://github.com/Jmgjava/team_project2/assets/154856565/136516e0-62cc-4601-94d3-694b24b2a92d) |

| 부서 삭제                                                                                                          |
|----------------------------------------------------------------------------------------------------------------|
| ![department_D](https://github.com/Jmgjava/team_project2/assets/154856565/53ede5f8-46bf-40c3-b797-5c91ab45ef0f) |

### chatBot

- 직원의 전화, 이메일, 부서 중 하나를 물어보면 그에 맞는 정보 텍스트로 전달

| 직원 검색                                                                                                            |
|------------------------------------------------------------------------------------------------------------------|
| ![chatBot_member](https://github.com/Jmgjava/team_project2/assets/154856565/884d7dae-8a61-4513-8d11-354b9040b740) |


<br>

![transparent](https://capsule-render.vercel.app/api?type=soft&color=324153&fontColor=fff&text=감사합니다.&animation=fadeIn&height=100&fontSize=40&descAlignY=80&descAlign=70)
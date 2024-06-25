# codingStory

<details>
<summary>2차 프로젝트 기본설정</summary>

프로젝트명 : codingStory

프로그래밍 언어 : JAVA

프레임워크 : Springboot 2.7.11

라이브러리 DI : Spring WEB(MVC), Thymeleaf, Spring Data JPA, Lombok, SpringSecurity5
, websocket, validation, OAuth2, security

데이터베이스 : MySql8

ORM : Spring Data JPA (JAVA(SQL))

개발툴 : IntelliJ

템플릿 엔진 : Thymeleaf (HTML + Data)

빌드 : Gradle

설정 : application.yml, application-oauth2.yml

</details>

![header](https://capsule-render.vercel.app/api?type=wave&color=auto&height=50px&section=header&text=개발자%20심지섭의%202차프로젝트&fontSize=50)

## 🔍목차 <br>
-[개요](#개요)<br>
-[프로젝트 상세](#프로젝트 상세내용)<br>

## 📝개요
<details>
<summary>프로젝트 개요</summary>
2차 프로젝트는 3차 프로젝트의 OPEN API를 연계하여 사용하기 위해 영화관으로 테마를 정했습니다.<br>
영화관에 근무하는 근무자들이 사용할 수 있는 관리자 페이지를 만들었고, 각종 기능들을 추가하였습니다.<br>
그 중 저는 근무자들이 보고서를 작성하고 결재를 받을 수 있게 하는 시스템을 만들었습니다. 

</details><br>


### <span style="color: white;">💻 프로그램 💻</span> <br>
<img src="https://img.shields.io/badge/notion-white?style=flat-square&logo=notion&logoColor=gray"/>
<img src="https://img.shields.io/badge/mysql-2E64FE?style=flat-square&logo=mysql&logoColor=white"/>
<img src="https://img.shields.io/badge/visualstudiocode-81BEF7?style=flat-square&logo=visualstudiocode&logoColor=blue"/>
<img src="https://img.shields.io/badge/intellijidea-navy?style=flat-square&logo=intellijidea&logoColor=white"/>
<img src="https://img.shields.io/badge/github-black?style=-square&logo=github&logoColor=white"/>

[//]: # (<img src="https://img.shields.io/badge/eclipseide-darkblue?style=flat-square&logo=eclipseide&logoColor=white"/>)

### <span style="color: white;">🛠 개발 환경 🛠</span> <br>
<img src="https://img.shields.io/badge/html5-green?style=flat-square&logo=html5&logoColor=white"/>
<img src="https://img.shields.io/badge/css3-blue?style=flat-square&logo=css3&logoColor=white"/>
<img src="https://img.shields.io/badge/auth0-ccc?style=flat-square&logo=auth0&logoColor=white"/>
<img src="https://img.shields.io/badge/chatbot-orange?style=flat-square&logo=chatbot&logoColor=white"/>
<img src="https://img.shields.io/badge/javascript-yellow?style=flat-square&logo=javascript&logoColor=white"/>
<img src="https://img.shields.io/badge/jquery-light?style=flat-square&logo=jquery&logoColor=white"/>
<img src="https://img.shields.io/badge/json-purple?style=flat-square&logo=json&logoColor=white"/>
<img src="https://img.shields.io/badge/openapiinitiative-FA5858?style=flat-square&logo=openapiinitiative&logoColor=white"/>
<img src="https://img.shields.io/badge/thymeleaf-0B610B?style=flat-square&logo=thymeleaf&logoColor=white"/>
<img src="https://img.shields.io/badge/spring-0B610B?style=flat-square&logo=spring&logoColor=white"/>
<img src="src/main/resources/static/images/readme/oAuth2.png" width="20" height="20"/> <br>

[![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=Sim)](https://github.com/Sim/github-readme-stats)
[![Anurag's GitHub stats](https://github-readme-stats.vercel.app/api?username=SIM)](https://github.com/SIM/github-readme-stats)




# 📁 프로젝트 상세

# 1. 보고서 문서 작성 후 결재자 설정<br>
## ● 보고서 작성 페이지
<img src="src/main/resources/static/images/readme/img.png"/>
● ↓ 작성자는 보고서 작성시 결재자를 선택할 수 있습니다. 선택할 때 동명이인을 구분하고 가독성을 높이기 위해 부서와 직급, 이름이 모두 보이도록 코드를 작성했습니다.<br>
    결재자의 정보는 데이터베이스에 저장된 회원들의 정보를 불러와 select option 으로 불러왔습니다.  <br> 

<img src="src/main/resources/static/images/readme/img_1.png"/> <br>

### ● 보고서의 종류
<img src="src/main/resources/static/images/readme/img_2.png"/><br>

### ● 부서 선택
부서는 관리자가 추가로 만들 수 있게 설계되어있습니다. 해당 부서들은 DB에서 데이터를 가져오는 것이기 때문에 부서가 추가된다면 해당 selectbox에도 자동으로 추가됩니다.<br>
<img src="src/main/resources/static/images/readme/img_3.png"/><br>

### ● 결재 기한 설정
<img src="src/main/resources/static/images/readme/img_4.png"/><br>

### ● 다른 데이터 베이스와 연관관계가 맺어져 있다.
<img src="src/main/resources/static/images/readme/img_5.png"/><br>
<img src="src/main/resources/static/images/readme/img_6.png"/><br>
<img src="src/main/resources/static/images/readme/img_8.png"/><br>

### ● 보고서 상신(상세보기) 페이지
<img src="src/main/resources/static/images/readme/img_9.png"/><br>
<img src="src/main/resources/static/images/readme/img_10.png"/><br>
상태의 값을 설정하여 상신을 누르게 되면 보고서의 상태값이 변화되어 저장됩니다.<br>
<br>

또한 결재 상신을 할 때 코멘트를 남길 수 있도록 textarea를 만들었으며, 작성 후 상신하면 코멘트 데이터가 저장되어 보고서 작성자에게 보이게 됩니다.
<img src="src/main/resources/static/images/readme/img_11.png"/><br>

### ● 보고서 리스트 페이지
보낸,반려된,결재 대기중,반려한, 전체 문서의 카테고리들을 나누어 페이지를 만들었는데 이동을 편리하게 하기 위해 상단에 버튼을 만들었습니다.
리스트에서는 사진과 같이 필요하다고 생각하는 데이터를 보여지게 하였습니다.
<img src="src/main/resources/static/images/readme/img_12.png"/><br>


### ● Index Main 페이지입니다.
로그인을 하면 본인에게 온 보고서가 있는지 한 눈에 파악하기 쉽도록 숫자로 표현하였습니다.
a태그를 통해 이동을 할 수 있도록 작성했습니다.
<img src="src/main/resources/static/images/readme/img_13.png"/><br>
<img src="src/main/resources/static/images/readme/img_14.png"/><br>

### ● Chat-Bot 페이지입니다.
사이드바 메뉴를 통해 '상담'을 클릭하면 Chat-Bot 페이지로 이동하게 됩니다.
해당 페이지의 좌측에는 자주하는 질문을 클릭하면 내려오는 드롭바 형식으로 만들었습니다.
<img src="src/main/resources/static/images/readme/img_15.png"/><br>
<img src="src/main/resources/static/images/readme/img_16.png"/><br>

<br>
우측의 상담문의 버튼을 누르면 Chat-bot 창이 뜨게 됩니다.
알고 싶은 회원의 이름과 정보를 검색하면 DB에서 정보를 가져와 사진처럼 출력을 합니다.
<img src="src/main/resources/static/images/readme/img_17.png"/><br>
<img src="src/main/resources/static/images/readme/img_18.png"/><br>



</details>

![Footer](https://capsule-render.vercel.app/api?type=waving&color=auto&height=200&section=footer)



[⬆⬆맨위로⬆⬆](#codingstory)<br>

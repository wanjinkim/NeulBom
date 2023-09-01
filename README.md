## 실버타운 그룹웨어 & 클라이언트 웹 프로젝트
### 주제
Servlet/JSP를 활용한 웹 프로젝트 구현

### 목적
- 효율적인 운영과 관리를 위한 관리자용 그룹웨어와 실버타운 통합 웹 페이지를 구현하고자 함
- 입주자들의 건강, 삶의 질, 사회 참여 등을 증진하기 위한 실버타운과 요양원을 운영하고,  다양한 서비스와 활동을 제공하기 위해 필요한 기능을 구상한다.
### 사용언어 & 사용기술
<img src="https://img.shields.io/badge/Java-007396?style=flat&logo=Java&logoColor=white" />  <img src="https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=HTML5&logoColor=white" />  <img src="https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=CSS3&logoColor=white" />  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=JavaScript&logoColor=black"/> <br>
<img src="https://img.shields.io/badge/Oracle-F80000?style=flat&logo=oracle&logoColor=white"/>  <img src="https://img.shields.io/badge/jQuery-0769AD?style=flat&logo=jquery&logoColor=white"/>  <img src="https://img.shields.io/badge/Bootstrap-7952B3?style=flat&logo=bootstrap&logoColor=white"/>   <img src="https://img.shields.io/badge/Chart.js-FF6384?style=flat&logo=chart.js&logoColor=white"/> <img src="https://img.shields.io/badge/Ajax-green?style=flat&logo=jquery&logoColor=white"/>  <img src="https://img.shields.io/badge/FlatPickr-blue?style=flat&logo=flatpickr&logoColor=white"/>

### 개발도구
<img src="https://img.shields.io/badge/Eclipse IDE-2C2255?style=flat&logo=eclipseide&logoColor=white"/>  <img src="https://img.shields.io/badge/Visual Studio Code-007ACC?style=flat&logo=visualstudiocode&logoColor=white"/>  <img src="https://img.shields.io/badge/Apache Tomcat-F8DC75?style=flat&logo=apachetomcat&logoColor=white"/>  <img src="https://img.shields.io/badge/Sourcetree-0052CC?style=flat&logo=sourcetree&logoColor=white"/> <img src="https://img.shields.io/badge/Git-orange?style=flat&logo=git&logoColor=white"/> <img src="https://img.shields.io/badge/Github-navy?style=flat&logo=github&logoColor=white"/> <img src="https://img.shields.io/badge/Exerd-red?style=flat&logo=exerd&logoColor=white"/> 

### 개발환경
<table>
  <tr>
    <td>OS version (platform)</td>
    <td>Windows(10, 11), Mac OS</td>
  </tr>
  <tr>
    <td>Language</td>
    <td>Java(OpenJDK 11.0.1), Oracle, HTML/CSS, JavaScript</td>
  </tr>
  <tr>
    <td>IDE</td>
    <td>SQL Developer, Exerd, Eclipse IDE 2021-03, Visual Studio Code, Source Tree</td>
  </tr>
  <tr>
    <td>DB</td>
    <td>Oracle Database 11g</td>
  </tr>
  <tr>
    <td>Server</td>
    <td>Apache Tomcat 8</td>
  </tr>
  <tr>
    <td>API, Library</td>
    <td>REST API(Kakao Map API, Daum Postcode API), jQuery, Chart.js, Flatpickr</td>
  </tr>
  <tr>
    <td>ETC</td>
    <td>BootStrap, Ajax, Git</td>
  </tr>
</table>

### 개요
1. 사용자는 관리자, 입주자, 보호자, 비회원으로 구분한다.
2. 관리자 그룹웨어와 입주자/보호자/비회원 클라이언트 페이지를 구분하여 제공한다.
3. 관리자는 계정 관리자, 일반 관리자, 그 외 직원으로 구분하고 권한별로 기능 접근 권한을 다르게 한다.

### 데이터 구조
![늘봄ERD(수정_0608_pm11 34)](https://github.com/wanjinkim/NeulBom/assets/45139754/41332e30-940f-493e-88aa-6f82a7df1fc4)


### 담당업무
- 메인화면 설계
- 회원가입
- 입주상담 게시판(조회, 등록, 수정, 삭제, 검색) 
---
### 화면구성
### 1. 메인화면 ⬇️
- header, 갤러리, footer로 이루어져있다.
- 메인 화면의 '로그인' 버튼을 클릭하여 로그인 페이지로 이동한다.
- 로그인은 '직원, 입주자, 보호자'로 구분하여 처리한다.

- **늘봄 소개** : 인사말, 시설소개, 오시는길
- **입주안내**
- **알림게시판** : 공지사항, 식단표, 생활게시판
- **커뮤니티** : 입주상담, 문의게시판, 자유게시판
![1-1  메인화면](https://github.com/wanjinkim/NeulBom/assets/45139754/a71069e2-3d11-4417-b913-081e4ed2c776)
![1-2  메인화면](https://github.com/wanjinkim/NeulBom/assets/45139754/68a77a32-b4b2-4683-b84a-906945621606)
![1-3  메인화면](https://github.com/wanjinkim/NeulBom/assets/45139754/022e7cd0-9885-4565-a476-80d535215afe)


### 2. 게시판 ⬇️
- 비회원은 입주상담 글을 등록, 조회, 수정, 삭제할 수 있다. 
- 비회원이 글을 작성하려면 이름과 전화번호를 입력받는다.
- **입력받은 정보와 일치하는 글만 조회, 수정, 삭제** 할 수 있다.
- 문의글에 관리자가 답변을 등록하고, 해당 글에는 **[답변완료]** 표시를 한다.
![4-2  비회원 입주상담](https://github.com/wanjinkim/NeulBom/assets/45139754/e45c4ad4-09f8-46b3-8cd7-9a925777c9e5)
![4-1  비회원 입주상담](https://github.com/wanjinkim/NeulBom/assets/45139754/c8c803e1-ffcd-4f64-a073-77681fc77556)


### 3. 관리자 - 재무관리 ⬇️
- chart.js를 사용하여 DB의 데이터와 연동된 차트를 출력한다.
- **원형차트** : 실버타운 입주자, 요양원 입주자 수를 표시
- **라인차트** : 최근 5개월 간의 지출 총액을 표시
- **최근지출내역** : 최근 10건의 지출 항목과 금액 등, 총 지출액 표시 
![3  재무관리](https://github.com/0hsoyeop/TW-Library/assets/131536077/9fc98612-c5a1-4078-a735-4b691446c4b2)

---
## 개발 스토리
### 회고
<table>
    <tr>
        <td>💡 기능구현 만큼 중요한 의견 통일, 코드 병합</td>
    </tr>
</table>
Servlet/JSP를 활용한 동적인 웹 페이지를 구현하는데 필요한 알고리즘이나 기능 구현에 어려움을 느끼긴 했으나, 
CRUD 기능을 수행하면서 이론 수업 진행 시 다소 헷갈렸던 doGet, doPost 방식의 데이터 전송 프로세스 및 
DB와의 연계 기능 특히 DAO, DTO, 웹 페이지 간 데이터를 주고받는 방법과 웹 페이지를 구현하는 과정에 대한 
이해도가 높아졌고 각자 목표로 한 기능들을 성공적으로 구현하였습니다.

그러나 문제는 의외의 곳에서 발생하였습니다, 프로젝트 초반 같은 기능을 목표로 하였으나, 
서로 생각하는 순서도, 기능 세부 조항이 다르다 보니 만들고 나서 서로의 기능이 얽혀있는 것이 아닌
따로따로 돌아가는 방식으로 구현되어 의견 통일을 하고 웹 페이지의 기능들을 통일하는 데 어려움을 겪었으며,

코드 병합 시 관리자 기능과 클라이언트 기능의 git 시작 시점이 달라 브랜치를 병합할 때 코드 일부가 충돌하거나 
이미 작업했던 코드가 사라지는 시행착오가 있었습니다. 이를 해결하기 위해 checkout으로 이전 코드를 가져와
손상된 파일을 다시 원래대로 복원하는 과정을 거쳤습니다.

이러한 경험을 통해 프로젝트 설계 단계 시 팀원들 간의 의견을 나누는 것과 코드를 병합 시키는 것은 기능 구현만큼
매우 중요하다는 것을 깨달았고, 앞으로의 프로젝트에서는 적극적인 의견 교환을 할 것이라 다짐했습니다.

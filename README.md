<p align="center">
<img src="img_read/logo.png">
</p>

# SIXMAN
## 02. 그룹웨어 기본 연동 기능 및 메시지 봇 구현 프로젝트
[프로젝트 소개 PPT(영상포함)](https://docs.google.com/presentation/d/1CkoOrN41lugsXsth9J_nlqLhLEDNJaqz/edit?usp=sharing&ouid=101047900780001156857&rtpof=true&sd=true)<br> 
[프로젝트 DB ERD](https://drive.google.com/file/d/1QUiq3_GKrSkSBKNos43bwLWZHIhj4pq9/view?usp=sharing)<br>

## 프로젝트 기간 
- 2023.09.26 ~ 2023.10.25

## 프로젝트 소개
- 학원을 기반으로 한 그룹웨어 페이지입니다.
- Spring MVC 패턴으로 개발하였습니다.
- 일정관리, 출결관리, 문서결재 기능구현 및 Naver API 연동을 추가하였습니다.
- Github Actions와 AWS EC2를 기반으로 CI/CD(지속통합/지속배포) 환경을 구축하였습니다.

## 개발 환경
- `Language` : Java 11, HTML5, CSS3, JavaScript
- `IDE` : IntelliJ IDEA, Visual Studio Code
- `Framework` : Springboot
- `Database` : MySQL
- `Template Engine` : Thymeleaf
- `ORM` : JPA <br>

## 팀 구성 및 역할
### 팀원 : 노승준 - 결재문서상세, CI/CD 구현
#### `Controller` : ApprovalController <br>`Templates` : Approval <br>

<details>
<summary>데이터 모델링 및 Entity, Dto 상세보기</summary>
<br>
  <p align="center"><img src="img_read/2ckDB.png"></p> 
<br>
  <p align="center">회원(employee)와 결재문서(approval)을 중심으로 전체적인 테이블과 연관관계를 설정하였고,</p>
  <p align="center">결재선(approval_user)을 추가로 구성하여 결재,참조 구분</p>
<br>
</details>
<br>
<details>
<summary>결재 문서 페이지(approval) 상세보기</summary>
<br>
  <p align="center"><img src="img_read/ap01.png"></p>
  <p align="center">결재 문서 작성 과정 중 문서를 결재하는 회원, 문서를 읽을 수 있는 회원 구분</p>
<br>
<br>
  <p align="center"><img src="img_read/ap02.png"></p>
  <p align="center">문서함 분류 상신함, 수신함, 결재함으로 설정</p>  
<br>
<br>
  <p align="center"><img src="img_read/ap03.png"></p>
  <p align="center">상신문서 결재하는 과정, 결재자로 지정된 사람만 버튼 확인 가능</p>  
<br>
</details>
<br>

<details>
<summary> CI/CD 구현 상세보기</summary>
<br>
  <p align="center"><img src="img_read/ap04.png"></p> 
<br>
</details>
<br>


#### 팀장 : 김** - 게시판상세, 공지사항상세, 프로젝트관리 <br>
#### 팀원 : 박** - 일정(FullCallendar API), 프론트엔드 <br>
#### 팀원 : 송** - 회원상세, Naver API <br>
#### 팀원 : 이** - 출결상세, 급여상세 <br>
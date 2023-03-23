##   🚀 서울컬쳐포트 (SeoulCulturePort)

📝 프로젝트 소개 : 서울시 문화 행사 검색과 리뷰 작성

📅 프로젝트 기간 : 2022.10.21-2022.10.27

👨‍👩‍👧‍👦  5조 : FE 송철환 김용민 , BE 장진혁 노명빈 [홍다정](https://github.com/bambee83)

# [![Youtube Badge](https://img.shields.io/badge/Youtube-ff0000?style=flat-round&logo=youtube&link=https://youtu.be/4bIADllM0B0)](https://youtu.be/4bIADllM0B0)   [![Notion Badge](https://img.shields.io/badge/Notion-000000.svg?&style=flat-round&logo=notion&link=https://www.notion.so/5-SA-f4ebf090ac43441f88ff063a6ee7cd78)](https://www.notion.so/5-SA-f4ebf090ac43441f88ff063a6ee7cd78) [![Web Badge](https://img.shields.io/badge/Web-EF5734.svg?&style=flat-round&logo=web&link=http://yongminbucket.s3-website.ap-northeast-2.amazonaws.com)]([https://www.notion.so/5-SA-f4ebf090ac43441f88ff063a6ee7cd78](http://yongminbucket.s3-website.ap-northeast-2.amazonaws.com)) 
<!--http://yongminbucket.s3-website.ap-northeast-2.amazonaws.com/-->

## 🔧 Technologies & Software Used

<img src="https://img.shields.io/badge/Spring-6DB33F?style=flat-round&logo=spring&logoColor=white"/>  <img src="https://img.shields.io/badge/SpringSecurity-6DB33F?style=flat-round&logo=SpringSecurity&logoColor=white"/>  <img src="https://img.shields.io/badge/SpringBoot-6DB33F?style=flat-round&logo=springboot&logoColor=white"/>  <img src="https://img.shields.io/badge/React-61DAFB?style=flat-round&logo=react&logoColor=white"/>    <img src="https://img.shields.io/badge/github-181717?style=flat-round&logo=github&logoColor=white"/>  

<img src="https://img.shields.io/badge/git-F05032?style=flat-round&logo=git&logoColor=white"/>  <img src="https://img.shields.io/badge/java-FF81F9?style=flat-round"/>  <img src="https://img.shields.io/badge/JSONWebToken-000000?style=flat-round&logo=JsonWebToken&logoColor=white"/>  <img src="https://img.shields.io/badge/Gradle-02303A?style=flat-round&logo=Gradle&logoColor=white"/>  <img src="https://img.shields.io/badge/IntelliJIDEA-000000?style=flat-round&logo=IntelliJIDEA&logoColor=white"/>  <img src="https://img.shields.io/badge/Postman-FF6C37?style=flat-round&logo=Postman&logoColor=white"/>  <img src="https://img.shields.io/badge/Notion-000000?style=flat-round&logo=Notion&logoColor=white"/>

<img src="https://img.shields.io/badge/AmazonS3-569A31?style=flat-round&logo=AmazonS3&logoColor=white"/>  <img src="https://img.shields.io/badge/AmazonEC2-FF9900?style=flat-round&logo=AmazonEC2&logoColor=white"/>  <img src="https://img.shields.io/badge/AmazonRDS-527FFF?style=flat-round&logo=AmazonRDS&logoColor=white"/>  <img src="https://img.shields.io/badge/MySQL-4479A1?style=flat-round&logo=MySQL&logoColor=white"/>  <img src="https://img.shields.io/badge/Ubuntu-E95420?style=flat-round&logo=Ubuntu&logoColor=white"/>

--react badge추가필요 ????

## ✨ 프로젝트 구현 기능 

1. 홈 화면 💒
  
  모든 사용자가 전체 게시글을 조회 및 검색을 할 수 있도록 구현하였습니다.
 
  회원가입과 로그인 을 헤더에 설정하여 로그인 시 마이페이지및 나의 닉네임을 확인할 수 있도록 하였습니다.  

2. 회원가입 로그인 🔑

   JWT + spring boot Security 를 적용하여 구현하였습니다.

3. 게시글 조회 📜

    최신순으로 조회할 수 있으며 전체 게시글, 상세 게시글, 마이페이지 게시글로 분류하였습니다. 

4. 게시글 작성 📝

    사용자가 업로드한 이미지를 Amazon S3로 저장하여 이미지 URL을 받아와 DB에 저장하여 관리합니다.
    
    작성자만 수정/ 삭제 할 수있으며 좋아요 기능이 포함되어 있습니다. 


5. 게시글 좋아요 💗

    사용자가 게시글에 좋아요를 누를 수 있고 다시 한 번 누르면 좋아요가 취소됩니다.

    상세 페이지의 경우 모든 사용자가 조회 가능 하지만, 로그인을 한 경우에만 좋아요를 누를 수 있습니다. 
    
6. 댓글 및 댓글 좋아요 💖

    게시글에 댓글을 작성할 수 있고, 작성자만 수정/ 삭제 할 수 있으며 게시글과 같이 좋아요 기능이 포함되어 있습니다.

7. 마이페이지 🌝

    내가 작성한 글, 댓글을 확인할 수 있습니다.

    해당 게시글의 상세페이지를 확인할 수 있습니다. 

8. 예외처리 📛

    Custom ErrorCode 및 statuscode를 전달하여 프론트엔드와 명확하게 소통하였습니다. 


## 🏀 Trouble Shooting

   Back-End
   1. 개인 계정마다 게시글, 댓글에 대한 좋아요 여부 판단 로직
   2. CICD 자동배포 민감한 정보 숨기기
   3. CORS 문제 해결
   4. API 명세서에 작성에 대한 중요성
  
   Front-End
  1. API 리퀘스트 변경에 대한 미숙지
  2. 로그인 시, 토큰 전송 방식으로 인한 이전 토큰 송신 문제
  3. dispatch 보낼 시 응답의 특정 조건에 따라 그 뒤 동작 달라지는 기능
  4. axios 요청 보낼 때 data-type


## 📋 API Table
|기능|method|URL|request|response|error code|
|:-----:|:---|:---|:---|:---|:---|
<!--
|홈|GET|/auth/home||{"goodWord": "팀원들과 예쁜말로 소통하고 있나요??","dday": -53}||
|중복확인|POST|auth/check|{“email” : "you1dsf"}|{"msg": "사용가능한 아이디입니다","statusCode": 200}|{"status": 400,"code": "AlreadyHaveEmail","message": "이미 존재하는 아이디 입니다."}{"status": 400,"code": "Size","message": "아이디는 4~12 개의 문자만 허용합니다."}|
|회원가입|POST|/auth/signup|{"email" : "you1dsf","accountName" : "짱윤서","accountPw" : "@weffs3424A","accountPwConfirm": "@weffs3424A","accountTeam": "3","accountLeader": false}|{"msg": "Success signup","statusCode": 200}|===비밀번호 조건이 부합하지 않을 때===[{"status": 400,"code": "NotBlank","message": "비밀번호는 공백일 수 없습니다."},{"status": 400,"code": "Size","message": "비밀번호는 8~!6 개의 문자만 허용합니다."},{"status": 400,"code": "Pattern","message": "비밀번호는 무조건 영문, 숫자, 특수문자를 각각 1글자 이상 포함해야 합니다."}]{"status": 400,"code": "NotMatchPassword","message": "비밀번호가 일치하지 않습니다."}|
|로그인|POST|auth/login|{"email" : "you1dsf","accountPw" : "@weffs3424A"}|{"msg": "Success Login","statusCode": 200}|{"status": 400,"code": "NotMatchPassword","message": "비밀번호가 일치하지 않습니다."}{"status": 400,"code": "NotFoundUser","message": "아이디가 존재하지 않습니다."}|
|게시글 작성|POST|api/posts|{img : ~~~.jpg, "title" : "제목입니다", "contents" : "내용입니다", "tag” : “일상”}|{"msg": "Success Post","statusCode": 200}||
|게시글 수정|PUT|api/posts/{postId}|img : ~~~.jpg, "title" : "제목입니다", "contents" : "내용입니다", "tag” : “일상”|{"modifiedAt": "2022-11-21T14:24:52.4777783"}|{"status": 400,"code": "NotMatchUser","message": "작성자가 일치하지 않습니다"}|
|게시글 삭제|DELETE|/api/posts/{postId}||{"msg": "게시글 삭제가 완료되었습니다!","statusCode": 200}|{"status": 400,"code": "NotMatchUser","message": "작성자가 일치하지 않습니다"}|
|게시글 좋아요|GET|api/{postId}/like||{    "success": true, "data": "게시글 좋아요 완료",“likesCount”: 2, "myError": null}||
|게시글 전체조회|GET|/api/posts?sort=createdAt&accountTeam=All&tag=All||{"postId": 4,"accountName": "짱윤서","title": "제목","contents": "내용","tag": "일상","comments": [],"postLikeCount": 1,"createdAt": "27분 전","modifiedAt": "21분 전","img": "https://mysparta4.s3.ap-northeast-2.amazonaws.com/testdir1/4762d4cf-8400-46df-b52e-944bbb3231f9KakaoTalk_20201226_121850849.jpg"}||
|우리조 게시글 조회하기|GET|/api/posts/myteam|{"postId": 4,"accountName": "짱윤서","title": "제목","contents": "내용","tag": "일상","comments": [],"postLikeCount": 1,"createdAt": "27분 전","modifiedAt": "21분 전","img": "https://mysparta4.s3.ap-northeast-2.amazonaws.com/testdir1/4762d4cf-8400-46df-b52e-944bbb3231f9KakaoTalk_20201226_121850849.jpg"}||
|댓글 작성|POST|api/{postId}/comments|{”comments”:”댓글입니다”}|{"postId": 2,"commentId": 3,"accountName": "짱윤서","comment": "댓글1","commentLikes": 0,"createdAt": "방금 전"}|{"status": 404,"code": "NotFoundPost","message": "게시물을 찾을 수 없습니다."}|
|댓글 삭제|DELETE|/api/{postId}/comments/{commentId}||{"data": "댓글 삭제가 완료되었습니다."}||
|댓글 좋아요|GET|/api/{postId}/comments/{commentId}/like||{"data": "댓글 좋아요 완료","likesCount": 1}||
|마이페이지 조회|GET|/api/myPage||{"accountName": "짱윤서","accountTeam": "3조","oneSentence": null,"myPost": [{"postId": 2,"accountName": "짱윤서","title": "제목","contents": "내용","tag": "일상","comments": [],"postLike": 1,"createdAt": "3분 전","modifiedAt": "2분 전","img": "https://mysparta4.s3.ap-northeast-2.amazonaws.com/testdir1/3fb27fd6-9e4e-420e-8cb0-633da85eee50KakaoTalk_20201226_121850849.jpg"},"myComment": [{"postId": 2,"commentId": 2,"accountName": "짱윤서","comment": "댓글1","commentLikes": 0,"createdAt": "3분 전"},]}||
|마이페이지 한줄 쓰기|POST|/api/myPage|{”oneSentence”:”짱성우다.”}|{"accountName": null,"accountTeam": null,"oneSentence": " 짱성우다.","myPost": null,"myComment": null}||
|마이페이지 한줄 수정|PUT|/api/myPage|{”oneSentence”:”저는 정성우가 아닙니다”}|{"accountName": null,"accountTeam": null,"oneSentence": " 저는 정성우가 아닙니다.","myPost": null,"myComment": null}||

-->

<!--

**Here are some ideas to get you started:**

🍿 Fun facts - what does your team eat for breakfast?
🧙 Remember, you can do mighty things with the power of [Markdown](https://docs.github.com/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
-->

## 프로젝트 이름

### STULS BOARD
<br><br>
## 프로젝트 소개


##### 첨부파일을 포함한 게시글을 올리는 간단한 게시판 프로젝트입니다.
##### 배포는 학습이 필요한 상황입니다.

## 개발환경

* IDE: IntelliJ IDEA Community
* Gradle - Groovy, Java 17
* Jar 11
* Spring Boot 2.7.6
* jvm.convert 3.3.2
* JDK 11
## 기술 스택

- HTML
- CSS
- JavaScript
- Lombok
- Thymeleaf
- Spring Data JPA
- Spring Web
- mysql 8.0.35

## 프로젝트 주요기능

#### 1. BOARD
 - 게시글생성
 - 게시글수정
 - 게시글조회
 - 게시글삭제
 - 페이징

#### 2. COMMENT
 - 댓글 작성
 - 댓글 목록
 - 댓글 수정
    - 댓글 내용
    - 댓글 작성자(추후 변경 예정)
 - 댓글 삭제
#### 3. FILE
 - 파일 저장
 - 파일 수정
 - 파일 다운로드
 - 파일삭제(현재 게시물을 삭제시에만 파일삭제)

---
|링크|기능|메소드|
|:--:|:--:|:--:|
|/board/create|게시글 작성페이지|Get|
|/board/save|게시글 저장|Post|
|/board/delete/{id}|게시글 삭제|Post|
|/board/paging/|게시글 목록|Get|
|/board/{id}|게시글 조회|Get|
|/board/update/{id}|게시글 수정페이지|Get|
|/board/update|게시글 수정|Post|
|/board/deleteFile/{fileId}|첨부파일 삭제|Post|
|/comment/save|댓글저장|Post|
|/comment/list/{boardId}|댓글목록|Get|
|/comment/update|댓글수정|Post|
|/comment/delete/{Id}|댓글삭제|Post|
|/download/{uuid}/{fileName}|파일 다운로드|Post|

파라미터
---
|작성중|작성중|작성중|
|:--:|:--:|:--:|

<br>
## 추후 업데이트 예정

##### 1. 회원가입, 로그인
##### 2. 인증,인가
##### 3. 게시글 내용에 첨부파일이 이미지일시 이미지 출력
##### 4. 페이지 스타일 변경
##### 5. 원하는 첨부파일만 삭제

# 버전


##### V1.2.3 (2023.12.16)
- [수정] 댓글 업데이트 오류 수정
- [수정] 페이지 로드시 댓글 출력
- [수정] 게시글 수정시 첨부파일이 있을때 첨부파일 없는상태로 저장시 기존파일 삭제 오류 수정
- [수정] 첨부파일 삭제 오류 수정
- [수정] 홈페이지 백그라운드 이미지 출력 오류 수정
- [오류] 원하는 첨부파일 삭제를 해도 삭제되지 않음

##### V1.2.2 (2023.11.30)
- [수정] 파일 업데이트 수정
- [수정] 파일 삭제 수정

##### V1.2.1 (2023.11.29)
- [수정] 게시글 수정 페이징 오류 수정
- [수정] 홈페이지 스타일 수정

##### V1.2.0 (2023.11.27)
- [추가] 댓글작성
- [추가] 댓글목록
- [추가] 댓글삭제
- [추가] 댓글수정
- [추가] 파일저장
- [추가] 파일삭제
- [추가] 파일다운로드
- [추가] 파일수정


##### V1.1.0 (2023.11.23)
- [생성] 게시글 삭제
- [생성] 게시글 조회
	- 게시글 번호
	- 제목
	- 작성일
	- 내용
- [생성] 게시글 수정
	- 게시글 제목
	- 게시글 내용
	- 수정날짜
- [생성] 게시판목록
	- 페이지 출력 게시글 5개
	- 페이지 수 3
- [생성] 홈페이지
	- 목록으로 이동
	- 글생성
	- <img src="/board/src/main/resources/static/readme/home.png">
##### V1.0.0 (2023.11.22)
- [생성] 게시글 생성
	- 제목
	- 내용
	- 작성일
	- 수정일

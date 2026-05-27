# -B2-
# 휴대폰 대리점 가격 비교 서비스
## 📱 내 주변 가장 저렴한 대리점 찾기
&nbsp;'CPC'는 내 주변 휴대폰 대리점(성지)의 실시간 시세를 비교하고, 지도에서 위치·경로를 확인하며, 사용자 후기를 공유할 수 있는 서비스입니다.

**모행 홍보 및 기능 설명 영상**

https://github.com/user-attachments/assets/d32ae2c1-c81e-4169-846c-e4f2d5d98933




## 🗒️목차
- [프로젝트 소개](#프로젝트-소개)
- [기능 설명](#기능-설명)
  - [화면 설명](#화면-설명)
  - [API 설명](#API-설명)
- [아쉬웠던 부분](#아쉬웠던-부분)

## 💻프로젝트 소개
프로젝트 이름: CPC ( 휴대폰 대리점 가격 비교 서비스 )

프로젝트 주제: 위치 기반 휴대폰 대리점 실시간 시세 비교 및 커뮤니티 앱

개발 인원 : 차우철, 최민식, 안재민, 김민호 

개발 형태: 정적 HTML/CSS/JavaScript 프론트엔드 프로토타입

배포 환경: 정적 리소스 (로컬 또는 정적 호스팅에서 구동)


>**기존의 문제점**
>
>&nbsp;휴대폰을 구매할 때 같은 기기라도 대리점(이른바 '성지')마다 조건과 가격이 크게 달라, 소비자가 발품을 팔지 않으면 합리적인 가격을 알기 어렵습니다. 시세 정보는 흩어져 있고, 요금제·보험 등 부가 조건이 가격에 어떻게 반영되는지 비교하기도 번거롭습니다.

>**해결 방법**
>
>&nbsp;제조사·모델·통신사 조건을 선택하면 주변 대리점의 시세를 한 화면에서 비교할 수 있도록 했습니다. 모델별 평균 시세, 거리·가격 정렬, 무한 스크롤 목록을 제공하고, 지도에서 대리점 위치와 경로(도보/차량)를 확인할 수 있습니다. 또한 커뮤니티를 통해 실제 구매 후기와 정보를 공유하여 정보 비대칭을 줄였습니다.

>**기대 효과**
>
>&nbsp;사용자는 불필요한 발품을 줄이고 합리적인 가격에 휴대폰을 구매할 수 있습니다. 후기와 정보 공유는 신규 사용자의 의사결정을 돕고 커뮤니티 유입을 유도하며, 가격 정보의 투명성이 높아져 건전한 시장 형성에 기여할 수 있습니다.

## ⚙️기능 설명
### 사용 기술
<div align=center><h3>📚 기술 스택</h3></div>
<div align=center> 
  <img src="https://img.shields.io/badge/html5-E34F26?style=for-the-badge&logo=html5&logoColor=white"> 
  <img src="https://img.shields.io/badge/css3-1572B6?style=for-the-badge&logo=css3&logoColor=white"> 
  <img src="https://img.shields.io/badge/javascript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black">
  <br>

  <img src="https://img.shields.io/badge/leaflet-199900?style=for-the-badge&logo=leaflet&logoColor=white">
  <img src="https://img.shields.io/badge/openstreetmap-7EBC6F?style=for-the-badge&logo=openstreetmap&logoColor=white">
  <br>

  <img src="https://img.shields.io/badge/github-181717?style=for-the-badge&logo=github&logoColor=white">
  <img src="https://img.shields.io/badge/git-F05032?style=for-the-badge&logo=git&logoColor=white">
</div>

### 메인 제공 기능
<div align=center> 
 
|로그인/회원가입|실시간 시세표|지도·경로|커뮤니티|마이페이지|
|------|------|------|------|------|
|`로그인.html` / `회원가입.html`|`리스트.html`|`지도맵.html`|`커뮤니티.html`|`프로필.html`|
|아이디·비밀번호 입력 후 진입 (데모용)|제조사·모델·통신사 필터, 정렬, 무한 스크롤, 상세 모달|Leaflet 지도에 주변 대리점 표시, OSRM 경로 안내|구매후기/질문답변/정보공유 게시판, 추천·최근순 정렬|상담 내역·관심 매장 등 사용자 메뉴|
</div>

**[화면 설명]** - 본 저장소는 정적 리소스 단일 프로젝트로, 각 `.html` 파일이 하나의 화면에 대응합니다.

**[API 설명]** - 별도의 백엔드 API가 없으며, 모든 데이터는 클라이언트에서 생성되는 목업 데이터입니다.

## 🔧아쉬웠던 부분
- 백엔드·데이터베이스 미구현으로 시세·게시글 등 모든 데이터가 목업으로만 동작
- 실제 인증 로직 없이 로그인/회원가입이 화면 흐름 시연용으로만 구현
- 시세 가격이 임의 공식과 랜덤 값으로 생성되어 새로고침 시 변동
- 지도 화면의 필터(제조사/모델/통신사)는 UI만 제공, 실제 필터링 미연동
- 검색 기능 및 게시글 상세/작성 화면 미구현
- 페이지마다 공통 CSS/JS가 분리되지 않고 중복

[화면 설명]: #메인-제공-기능
[API 설명]: #API-설명

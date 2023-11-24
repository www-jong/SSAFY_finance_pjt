# **[*FINAL PJT* - 금융 상품 비교 애플리케이션]**

# 💵 <mark>더쓸라 (THESLA)</mark>

> ## 🧭 프로젝트 개요

- 이 프로젝트는 금융 상품 비교를 위한 웹 애플리케이션을 제작한 것입니다.

- 예금 및 적금 금리를 비교하고 데이터 분석을 통해 사용자에게 적합한 금융 상품을 추천할 뿐만 아니라, 그 외에도 사용자의 다른 금융 활동들의 편의를 위한 기능과 정보들을 제공합니다. 

---

> ## 👥 팀 소개

- 원종현
  
  - (역할 쓰기)

- 김민진
  
  - (역할 쓰기)

---

> ## ❗ 더쓸라 로고

(로고 이미지)

---

> ## 🪢 배포 URL

asfsaf

---

> ## 💎 메인 기능

- 예금 및 적금 금리 비교

- 환율 계산기

- 내 집 주변 은행 검색

- 나에게 맞는 상품 추천

- ```완성본
  
  ```

---

> ## ✅ 프로젝트 요구 사항

- 메인 페이지
  
  - 서비스 소개 및 메인 페이지 구성

- 회원 커스터마이징
  
  - 회원 관리 기능 구성 (회원 가입, 로그인, 로그아웃 등)

- 예적금 금리 비교
  
  - 데이터 저장
    
    - 적절한 API를 활용하여 금융 상품 데이터를 DB에 저장
  
  - 전체 조회
    
    - 상품 목록을 조회할 수 있는 화면 구성
    
    - 은행을 선택하여 목록을 필터링할 수 있도록 추가 기능 구성
  
  - 상세 조회
    
    - 해당 금융 상품에 대한 자세한 정보를 출력할 수 있는 화면 구성
    
    - 관리자는 금리 정보를 수정할 수 있도록 구현
    
    - 상품의 금리 정보가 수정되면 가입한 유저의 이메일로 메일이 전송되도록 구현

- 환율 계산기
  
  - 적절한 API를 활용하여 현재 환율에 대한 정보 가져오기
  
  - 국가를 선택할 수 있도록 구성
  
  - 원화 입력 시, 선택한 국가의 통화로 변환된 값을 출력
  
  - 타국 통화 입력 시, 해당 통화를 원화로 변환한 값을 출력

- 근처 은행 검색
  
  - 적절한 API를 활용하여 지도를 표시
  
  - 위치와 은행을 선택할 수 있도록 구성

- 커뮤니티 (게시판)
  
  - 회원 간 소통할 수 있는 커뮤니티 기능(게시판)을 구현
  
  - 게시글 조회, 생성, 삭제, 수정 구현
  
  - 댓글 생성, 삭제 기능 구현
  
  - 회원의 권한에 따라 다른 동작을 하도록 구성

- 프로필 페이지
  
  - 회원의 기본 정보를 출력할 수 있도록 적절한 화면 구성
  
  - 회원의 정보를 수정하기 위한 적절한 화면 구성
  
  - 내가 가입한 금융 상품 리스트를 출력하는 화면 구성
  
  - 차트 라이브러리를 활용하여 가입한 상품 금리 정보를 그래프로 출력

- 금융 상품 추천 알고리즘
  
  - 사용자에게 적합한 금융 상품을 추천할 수 있는 알고리즘 구현

---

> ## 🔥 더쓸라의 추가 구현 기능

- aaaa
  
  - bbb

---

> ## 🖥️ 개발 환경

- **OS**
  
  - Windows (10, 11)

- **IDE**
  
  - Visual Studio Code (1.84.2)

- **Programming Language**
  
  - Python (3.9.13)
  - JavaScript (ES6+)

- **Front-end Framework**
  
  - Tailwind CSS (3.3.2)
  
  - Vue.js (3.3.4)

- **Back-end Framework**
  
  - Django (4.2.4)

- **Library**
  
  - Node.js (20.9.0)
  
  - Django REST framework (3.14.0)

- **DBMS**
  
  - SQLite (3.44.0)

---

> ## 📑 API

- 금융감독원 금융상품통합비교공시
  
  - 정기예금상품 API, 적금상품 API

- 한국수출입은행
  
  - 현재환율 API

- 카카오
  
  - 지도 API

- 네이버
  
  - 뉴스 검색 API

---

> ## 🏗️ 개체-관계 다이어그램 (ERD)



---

> ## 📚 컴포넌트 다이어그램

![](C:\Users\SSAFY\AppData\Roaming\marktext\images\2023-11-24-09-39-25-image.png)

---

> ## ✨ 금융 상품 추천 알고리즘
### 사용자 기반 코사인 유사도를 이용한 협업 필터링 추천(Collaborative Filtering)
- 개념
  - 많은 사람들의들의 나이, 소득, 자산 및 금융상품 선호도를 통해 나와 유사한 사람들이 선호하는 금융상품을 추천
- 사용자 기반 유사도 측정(코사인 유사도)
  ![algo](https://github.com/www-jong/SSAFY-finance-pjt/assets/88592432/23b38572-8564-4f4b-b9cb-69fa2ffba2ba)
  - 두 벡터의 코사인각도를 계산해 유사성 측정
  - 즉, 구하고자 하는 사람의 금융상품 선호도(추천)과 사람들을 1:1로 코사인유사도를 구해 금융상품 선호도 우선순위 설정
- 사용한 유저데이터
  - 더미데이터를 통해 구현
  - 3만명의 랜덤한 유저데이터를 이용함
  - 랜덤하게 설정된 나이, 재산, 소득, 선호하는 금융상품을 통해 구현
---

> ## 🍀 프로젝트 후기

- 원종현
  
  - SSAFY에서 처음 진행한 팀프로젝트이며, 1학기의 마무리를 알리는 관통프로젝트였습니다. 약 일주일의 길지도않고 짧지도않은 시간이었지만 지금까지 배워왔던 기술들을 한번씩 다 활용해 볼 수 있는 좋은 기회였고, 부족한 팀프로젝트 경험을 쌓을 수 있는 기회였습니다. 그리고 또 한번 ,기획의 중요성을 깨닫게 되는 프로젝트였습니다.  여러 어려움이 많았고, 답답함도 많았지만 이리저리 부딫히면서 최대한 구현해낼 수 있을만큼 구현을 해서 조금은 후련합니다. 그리고 뭐니뭐니해도 디자인이 가장 어렵다는 것을 깨달았습니다. 기술스택말고도, 디자인스택(?)도 소홀히 하지 않아야겠습니다. 일주일 동안 같이 고생한 페어 민진이형 정말 수고했고 고생하셨습니다!

- 김민진
  
  - ㅁㄴㅇㄹ

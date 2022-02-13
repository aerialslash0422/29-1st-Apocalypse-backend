# 29-1st-Apocalypse-Backend

## Introduction
포스트 아포칼립스에 걸맞는 상품들을 판매하는 커머스 사이트 __종말론__ 구현

향수 판매 커머스 사이트인 [조 말론](https://www.jomalone.co.kr/)의 클론 코딩 프로젝트입니다.


## 개발 인원 및 기간
- 기간 : 21.01.24 ~ 22.02.11
- Frontend 4명 : 김기만, 박재형, 이화종, 홍지은
- Backend  2명 : 김준영, 이강일
- 
[Backend Git Repository](https://github.com/wecode-bootcamp-korea/29-1st-Apocalypse-backend)

[Frontend Git Repository](https://github.com/wecode-bootcamp-korea/29-1st-Apocalypse-frontend)

## 적용 기술 및 구현 기능
- `Frontend`       : JavaScript, React.js, SASS, React-router-dom
- `Backend`        : Python, Django, MySQL, AWS(EC2, RDS, S3)
- `협업 및 일정 관리` : Git, Github, Slack, Trello, Notion


## Reference
[API Documentation](https://documenter.getpostman.com/view/19473444/UVeJKkH6)

[db.diagram](https://dbdiagram.io/d/61ee2a5b7cf3fc0e7c59b78f)


## 프로젝트에서 내가 담당/작업했던 기능들

#### User API
- Validation, 인증/인가 모듈화 초안 코드리뷰 받고 수정

#### Product API
- 전체 카테고리, 서브카테고리(대분류,소분류)
- 상품 리스트, 키워드를 통한 상품 정렬(sorting) 및 검색(영문,한글이름)
- 상품 상세 정보 `Path Parameter` 수정  

#### Cart API
- 장바구니 조회(GET) 기능에서 `aggregate`를 이용한 장바구니에 담긴 상품의 가격 총 합계 구현 도움

#### Order API
- 주문하기

장바구니 Data를 들어와 주문/주문상품 Table에 추가(POST), 장바구니 Table Data 삭제(DELETE), Transaction을 통한 무결성 보장
- 주문 내역 조회(GET)
- 주문 취소(PATCH) - 주문/주문상품 Status 변경, Transaction을 통한 무결성 보장

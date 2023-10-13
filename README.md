# flavor-match 

세계의 많은 사람들의 문화, 종교, 신념, 취향 등이 서로 다르고 더욱 세분화되고 있으나, 이 모든 요구를 수용하는 식당을 찾기 어려워서 이 문제를 해결하기 위해
글로벌 사용자들의 요구를 수용할 수 있는 음식점 추천 어플 구현

## 화면 설계

## 기능 명세서

## 시스템 아키텍처

## ERD

## 개발 환경

## 서비스 흐름도

## API 목록
### VIEW
| 종류 | URL         | Method | Description            | 기타         |
|------|-------------|--------|------------------------|--------------|
| 뷰   | `/`         | GET    | 루트 페이지             |              |
|      | `/error`    | GET    | 에러 페이지             |              |
|      | `/login`    | POST   | 로그인 페이지           |              |
|      | `/sign-up`  | GET    | 회원가입 페이지         |              |
|      | `/mypage`   | GET    | 개인정보 페이지         |              |
|      | `/myreviews`| GET    | 내가 쓴 리뷰 페이지     |              |
|      | `/myfavorites`| GET  | 내가 좋아요를 누른 식당 페이지 |      |
|      | `/restaurants`| GET  | 식당정보 페이지         |              |

### DATA
| 종류 | URL                                                   | Method    | Description                        | 기타             |
|------|-------------------------------------------------------|-----------|------------------------------------|------------------|
| API  | `/api/login`                                          | POST       | 회원 로그인                        |                  |
|      | `/api/mypage/{user-id}`                               | GET       | 회원 정보 조회                     |                  |
|      | `/api/mypage`                                         | POST      | 회원 정보 입력                     |                  |
|      | `/api/mypage/{user-id}`                               | PUT, PATCH| 회원 정보 수정                     |                  |
|      | `/api/mypage/{user-id}`                               | DELETE    | 회원 탈퇴                         | 로직 변경 필요   |
|      | `/api/myreviews/{user-id}`                            | GET       | 회원이 작성한 리뷰 리스트 조회     |                  |
|      | `/api/restaurants`                                    | POST      | 식당 리스트 검색                   |                  |
|      | `/api/restaurants/{restaurant-id}`                    | GET       | 단일 식당 상세정보 조회            |                  |
|      | `/api/restaurants/{restaurant-id}`                    | POST      | 식당 상세정보 입력                 | 비즈니스 고객?   |
|      | `/api/restaurants/{restaurant-id}`                    | PUT, PATCH| 식당 상세정보 수정                 | 비즈니스 고객?   |
|      | `/api/restaurants/{restaurant-id}`                    | DELETE    | 식당 상세정보 삭제                 | 비즈니스 고객?   |
|      | `/api/myfavorites/{user-id}`                          | GET       | 회원 북마크 조회                   | 식당 대시보드   |
|      | `/api/myfavorites/{user-id}/{restaurant_id}`          | GET       | 북마크한 식당 단일 조회            |                  |
|      | `/api/restaurantComments`                             | GET       | 식당 리뷰 조회                     |                  |
|      | `/api/restaurantComments/{restaurant-comment-id}`     | GET       | 식당 리뷰 단일 조회                |                  |
|      | `/api/restaurants/{restaurant-id}/restaurantComments` | GET       | 식당에 연관된 댓글 리스트 조회     |                  |
|      | `/api/restaurants/{restaurant-id}/restaurantComments/{restaurant-comment-id}`| GET | 식당에 연관된 댓글 조회 |          |
|      | `/api/restaurants/{restaurant-id}/restaurantComments` | POST      | 댓글 등록                          |                  |
|      | `/api/restaurants/{restaurant-id}/restaurantComments/{restaurant-comment-id}`| PUT, PATCH| 댓글 수정  |          |
|      | `/api/restaurants/{restaurant-id}/restaurantComments/{restaurant-comment-id}`| DELETE | 댓글 삭제  |          |


##TEST

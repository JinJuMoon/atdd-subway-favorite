# 즐겨찾기 - API 테스트/문서자동화

# 🤔 미션 소개

## 미션 목적

- 인수 테스트 작성 후 병렬 작업 수행과 프론트 협업을 위한 문서 자동화 학습
- 인수 테스트와는 별개로 API 요청별 응답을 각각 테스트 하기 위한 통합 API 테스트를 학습
- 로그인 기능 구현을 통한 로그인 프로세스 경험

![https://techcourse-storage.s3.ap-northeast-2.amazonaws.com/2020-05-03T17%3A08%3A24.123image.png](https://techcourse-storage.s3.ap-northeast-2.amazonaws.com/2020-05-03T17%3A08%3A24.123image.png)

## 미션 주제

- 회원관리 / 즐겨찾기 기능

# 1단계 - 회원관리 기능

## 요구 사항

- 회원 정보를 관리하는 기능 구현
    1. 회원가입
        - [x] 인수 테스트 작성
        - [x] 단위 테스트 작성
        - [x] API 문서를 작성하고 문서화를 위한 테스트 작성
        - [ ] side case에 대한 예외처리
        - [x] 페이지 연동
    2. 로그인
        - [x] 인수 테스트와 단위 테스트 작성
        - [x] API 문서를 작성하고 문서화를 위한 테스트 작성
        - [x] 토큰의 유효성 검사와 본인 여부를 판단하는 로직 추가
            - [x] JWT 방식 활용
        - [x] side case에 대한 예외처리
        - [x] 페이지 연동
    3. 로그인 후 회원정보 조회/수정/삭제
        - [x] 인수 테스트 작성
        - [ ] 단위 테스트 작성
            - [x] 컨트롤러 단위 테스트
            - [ ] 서비스 단위 테스트
        - [x] API 문서를 작성하고 문서화를 위한 테스트 작성
        - [x] 토큰의 유효성 검사와 본인 여부를 판단하는 로직 추가
            - [x] 자신의 정보만 수정 가능하도록 해야하며 **로그인이 선행**되어야 함
            - JWT 방식 활용
        - [ ] side case에 대한 예외처리
        - [x] 페이지 연동
        
# 2단계 - 즐겨찾기 기능

## 요구사항

- 즐겨찾기 기능 구현
    1. 즐겨찾기 추가
        - [x] 인수 테스트 작성
        - [x] 단위 테스트 작성
            - [x] 컨트롤러 단위 테스트
            - [x] 서비스 단위 테스트
        - [ ] API 문서를 작성하고 문서화를 위한 테스트 작성
        - [x] 즐겨찾기 추가 기능을 구현
            - 자신의 즐겨찾기만 추가 가능
            - 토큰의 유효성 검사와 본인 여부를 판단하는 로직 추가(interceptor, argument resolver)
        - [ ] side case에 대한 예외처리 필수
            - [ ] 중복된 즐겨찾기를 추가하려고 할 경우 예외 발생
        - [ ] 페이지 연동
    2. 즐겨찾기 목록조회 / 제거
        - [x] 인수 테스트 작성
        - [x] 단위 테스트 작성
            - [x] 즐겨찾기 목록조회 - 컨트롤러 단위 테스트
            - [x] 즐겨찾기 목록조회 - 서비스 단위 테스트
            - [x] 즐겨찾기 삭제 - 컨트롤러 단위 테스트
            - [x] 즐겨찾기 삭제 - 서비스 단위 테스트
        - [ ] API 문서를 작성하고 문서화를 위한 테스트 작성
        - [x] 즐겨찾기 목록조회 / 제거 기능을 구현
            - [x] 즐겨찾기 목록조회 기능 구현
            - [x] 즐겨찾기 제거 기능 구현
            - 자신의 즐겨찾기만 조회/삭제 가능
            - 토큰의 유효성 검사와 본인 여부를 판단하는 로직 추가(interceptor, argument resolver)
        - [ ] side case에 대한 예외처리 필수
        - [ ] 페이지 연동

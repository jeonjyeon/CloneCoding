# 아토믹 디자인 기반 넷플릭스 클론코딩 (HTML, CSS)

## 1. 아토믹 디자인 (Atomic Design)이란?

> 디자인 시스템을 체계적으로 구성하는 방법론

## 2. 아토믹 디자인의 구조와 의미

    원자(Atomics) → 분자(Molecules) → 유기체(Organisms) → 템플릿(Templates) → 페이지(Pages)

| 단계      | 설명                                                                   |
| --------- | ---------------------------------------------------------------------- |
| Atomics   | 텍스트, 버튼, 입력창 등 가장 기본적인 UI 단위 요소                     |
| Molecules | 두세 개의 Atoms를 조합한 소규모 컴포넌트 (예: 라벨 + 인풋 필드 + 버튼) |
| Organisms | 여러 Molecules가 모여 구조를 갖춘 독립적 블록 (예: 헤더, 푸터)         |
| Templates | Organism들을 배치해 전체 레이아웃 구조를 설정한 틀                     |
| Pages     | 템플릿에 실제 데이터를 넣어 실제 UI처럼 보이게 한 화면                 |

## 3. 진행 단계

1. 디자인 분석

   - 넷플릭스 UI를 보고 원자 단위로 분해

     → 텍스트, 아이콘 버튼, 썸네일 카드, 탭 메뉴 등

2. Atomics 만들기

   - 넷플릭스 UI 스크린샷을 분석해 가장 작은 단위로 분해
   - 예시 구성 요소: button, input, title, icon, 등
   - 단순 스타일만 적용

3. Molecules 만들기

   - 기본 단위 UI 요소 정의
   - 예시: SearchBar = input + button
   - Atoms를 묶어서 기본 상호작용 만들기

4. Organisms 만들기

   - 여러 Molecules가 모여 의미 있는 블록을 구성
   - 예시: Header, MovieCarousel, Footer 등

5. Templates 구성

   - Organisms들을 레이아웃 구조에 맞게 배치
   - 예시: MainTemplate = Header + Main + Footer

6. Pages 구현
   - Template에 실제 콘텐츠 데이터 넣어 최종 화면 구성
   - 예시: 영화 썸네일 이미지, 영화 제목 및 설명, 사용자 정보 등

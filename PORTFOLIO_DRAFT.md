# 혁의 사용자 가이드 ヒョクのユーザーガイド

세로쓰기 한·일 병기 타이포그래피로 구성한 개인 인덱스 페이지. 매 접속마다 색상과 4분할 레이아웃이 무작위로 재배치되는 정적 단일 페이지다.

## 서술

화면은 좌상·우상·좌하·우하 4개 구획으로 나뉘며, 각 구획에 자기소개 목록, 마방진(魔方陣) 표, 외부 작업 링크, 참고 출처가 배치된다. `script.js`는 페이지 로드 시 6개의 색상 조합 중 하나를 무작위로 골라 CSS 변수 `--color-2`·`--color-3`에 주입하고, Fisher-Yates 셔플로 네 구획의 위치를 섞어 매번 다른 배열을 만든다. 타이포그래피는 `writing-mode: vertical-rl` 기반의 세로쓰기를 전반에 적용하고, Adobe Fonts(고즈카명조·AG최정호)와 Pretendard·부크크명조 웹폰트를 CDN으로 불러와 한글과 일본어·한자를 함께 조판한다. 프레임워크나 빌드 도구 없이 HTML·CSS·바닐라 자바스크립트 세 파일로만 구성했고, 표 그래픽은 페이지 본문에 명시된 대로 Kohei Sugiura의 『印刷ユーザーガイド』에서 영향을 받았다.

## 스펙

- **역할**: 개인 작업 — 디자인 및 프론트엔드 구현 (단독)
- **스택**: HTML, CSS, Vanilla JavaScript (프레임워크·빌드 도구 없음)
- **주요 의존성**:
  - Adobe Fonts / Typekit (kit `hvw8xwa`) — `kozuka-mincho-pr6n`, `agchoijeongho-screen`, `optique-display`
  - Pretendard (jsDelivr CDN, `@import`)
  - 부크크명조 BookkMyungjo (projectnoonnu noonfonts, woff2)
- **규모**: 3개 파일 — `index.html`, `script.js`(약 42줄), `style.css`(약 297줄), 단일 페이지
- **링크**:
  - 라이브: https://h2j603.github.io/home/ (GitHub Pages, 추정)
  - 리포: https://github.com/h2j603/home

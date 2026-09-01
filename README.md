# 🎂 Birthday Hacking Protocol

해킹/기밀 접근 컨셉의 인터랙티브 생일 축하 웹앱입니다.
순수 HTML/CSS/JavaScript로만 작동하며, 외부 라이브러리가 필요 없습니다.

## 사용 방법

1. 이 저장소를 GitHub Pages로 배포합니다.
2. 생성된 링크를 열면 바로 시작됩니다.
3. 모바일 브라우저에 최적화되어 있습니다.

## 진행 흐름

1. **접근 경고 화면** — 시스템 강제 접속 시도
2. **패스코드 입력** — 4자리 숫자 키패드
3. **로봇 배 메시지** — 안내 문구
4. **미션 1** — 케이크 초 개수 맞히기 (객관식)
5. **미션 2** — 연도 맞히기 (숫자 입력, 지하철 첫 만남 애니메이션)
6. **FINAL CHECK** — 힌트 확인 준비
7. **열쇠 팝업 → 보석함** — 선물 힌트 공개
8. **정답 제출** — 선물이 무엇인지 주관식 입력
9. **엔딩** — 로봇의 작별 인사

## 커스터마이징

`index.html` 안의 `<script>` 상단 `CUSTOMIZATION ZONE`에서 아래 값들을 수정할 수 있습니다.

```js
const PASSCODE    = "0908";          // 패스코드 (MMDD)
const TARGET_NAME = "KIM_YOUNGBIN";  // 파일명에 쓰일 이름
const BUDDY_NAME   = "꽁꽁이";        // 로봇 이름

const BUDDY_LINES = { ... };  // 화면별 로봇 대사
const GIFT_HINT   = `...`;    // 보석함 힌트 문구
```

미션의 정답, 문구, 애니메이션 등은 `index.html` 내부에서 직접 수정 가능합니다.

## 파일 구성

```
index.html   전체 앱 (HTML + CSS + JS)
README.md    이 문서
```

## 기술 스택

- HTML5 / CSS3 (애니메이션, Flexbox)
- Vanilla JavaScript (외부 라이브러리 없음)
- SVG (일러스트 및 캐릭터)

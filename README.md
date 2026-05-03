# 부송 배드민턴 클럽 20주년 — 메인 아카이브 (v2.0)

## 📂 폴더 구조

```
busong-main/
├── index.html                       (60 KB · EP 통일 디자인)
├── README.md                        이 파일
├── photos/                          82장 / 약 6.8 MB
│   ├── 2007-01.jpg ~ 2026-01.jpg    81장 (연도-순번)
│   └── finale-2025-inauguration.jpg 피날레 1장
└── audio/
    └── bgm.mp3                      꿈을 꾼다 - 서영은 (4.5 MB)
```

## 🎨 EP1~4 시리즈와 통일된 디자인 시스템

| 토큰 | 값 | 용도 |
|---|---|---|
| `--navy` | `#0D1B33` | 메인 배경 |
| `--navy-deep` | `#08101F` | 깊은 배경 |
| `--navy-mid` | `#1A2A45` | 카드/섹션 |
| `--gold` | `#C9A961` | 메인 골드 |
| `--gold-bright` | `#F0C870` | 강조 골드 |
| `--serif` | Noto Serif KR | 제목 |
| `--sans` | Pretendard | 본문 |

## 🔗 외부 링크 구성

### EP 시리즈 카드 (4개)
- EP1 「창립의 열정」 → `https://manminkim-eng.github.io/Busong-Club-20th-Ep01/`
- EP2 「함께 자란 시간」 → `https://manminkim-eng.github.io/Busong-Club-20th-Ep02/`
- EP3 「역사를 잇다」 → `https://manminkim-eng.github.io/-Busong-Club-20th-Ep03/` ⚠️ 앞 하이픈
- EP4 「그래도, 부송」 → `https://manminkim-eng.github.io/Busong-Club-20th-Ep04/`

### 영상 링크
- 메인 종합영상: https://youtu.be/SF9k0U0KqrY (7분)
- 회원모집 숏츠: https://youtube.com/shorts/54f1iakXK2k

## 🎯 페이지 구성 (스크롤 순서)

1. **INTRO** — 풀스크린 시작 화면 (▶ 브이로그 시작 버튼)
2. **BGM 컨트롤** — sticky 상단 바 (꿈을 꾼다 - 서영은)
3. **HERO** — 부송 배드민턴 클럽 + 셔틀콕 점 애니메이션
4. **STATS** — 20년 / 20기 / 14명 (카운트업)
5. **EP 시리즈 카드 4개** ⭐ NEW — YouTube 썸네일 자동 로드
6. **TIMELINE** — 2007~2026 연도별 사진 81장
7. **역대 회장단** — 14명 그리드
8. **FINALE** — 19·20기 김종왕 회장 이취임식 사진
9. **메인 종합영상 CTA** — 6개 챕터 마커 + 빨간 버튼
10. **회원모집 숏츠 CTA** ⭐ NEW — 카드 형태 (썸네일 + 정보)
11. **푸터** — 슬로건 + 주최자 정보

## 🛡️ 사진 링크 오류 방지 (8중 안전망)

- ✅ URL-safe 파일명 (영문 소문자 + 숫자 + 하이픈만)
- ✅ Linux/GitHub Pages case-sensitive 환경 호환
- ✅ 모든 `<img>`에 `loading="lazy"` + `decoding="async"`
- ✅ `onerror` 폴백 — 누락 시 친절한 안내 메시지
- ✅ 라이트박스에도 `onerror` 처리
- ✅ 양방향 검증 통과 (참조 83개 ↔ 실파일 83개)
- ✅ JPG/MP3 시그니처 검증 통과
- ✅ 파일명 충돌 없음

## 🎵 BGM UX (EP1~4와 동일 패턴)

1. 첫 진입 시 **음소거 자동재생** 시도
2. 사용자 첫 클릭/터치 시 **소리 unlock**
3. 우상단 **인디케이터** (이퀄라이저 애니메이션)
4. **토스트 알림** (음소거 시 펄싱 효과)
5. **localStorage**에 사용자 BGM 선호 기억 (`busong_main_bgm_pref`)

## 📊 용량 비교

| 항목 | 변경 전 (단일 HTML) | 변경 후 (분리) |
|---|---|---|
| **단일 파일** | 15.0 MB | 60 KB |
| **첫 진입 시 다운로드** | 15.0 MB | **60 KB + lazy load** |
| **사진** | 미리 다 받음 | 스크롤 시 필요한 만큼만 |
| **BGM** | 인라인 base64 | 별도 파일 (캐시) |

## 📌 사진 추가/교체 가이드

- 새 사진: `photos/2027-01.jpg` 형식으로 저장 → `index.html`의 `PHOTOS` 배열에 추가
- 사진 교체: 같은 파일명으로 덮어쓰기 → 브라우저 새로고침 (Ctrl+Shift+R)
- 금지: 한글 파일명, 공백, 괄호, 물음표, 대문자 확장자

## 🌐 GitHub Pages 배포

`Busong-Club-20th-Anniversary/` 저장소 루트에 폴더째 업로드 → 자동 인덱스 표시

---
**부송 배드민턴 클럽** · 창립 2007년 1월 · 20주년 영상 시리즈 기획 총괄: 김만민 남부회장

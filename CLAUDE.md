# 규칙

- 결과값과 설명은 한글로 작성한다.

---

## Design

| 항목 | 값 |
|------|----|
| 해상도 | 800×1280, 반응형 |
| Primary 컬러 | `#122961` (진한 네이비) |
| Secondary 컬러 | `#FCE300` (옐로우) |
| 명도대비 | 4.5:1 (일반) / 3:1 (30px 이상 텍스트) |
| 아이콘 | 텍스트와 함께 항상 제공 |
| 최소 터치영역 | 48×48px |
| 요소 간 간격 | 최소 20px |
| 폰트 | `-apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif` |
| 폰트 굵기 | 최대 700 |
| 레이아웃 | 주요 액션 단순 노출, 서브 텍스트 절제 |

### CSS 변수
```css
:root {
  --color-primary:       #122961;
  --color-primary-dark:  #0A1A42;
  --color-secondary:     #FCE300;
  --color-secondary-dark:#D4BD00;
  --color-bg:            #F5F5F5;
  --color-surface:       #FFFFFF;
  --color-text-primary:  #111111;
  --color-text-on-primary: #FFFFFF;
  --color-text-on-secondary: #111111;
  --color-border:        #CCCCCC;
  --color-success:       #1A6B2A;
  --color-hint:          #122961;
  --min-touch:           48px;
  --gap:                 20px;
}
```

---

## UX Guide

1. **단순한 화면** — 화면당 주요 행동 1~2개, 서브 텍스트 최소화
2. **명시적 피드백** — 담기, 결제 등 주요 행동 완료 후 명확한 확인 메시지 표시
3. **명확한 취소/뒤로가기** — 모든 화면 좌상단 고정, 레이블 포함
4. **부정적 단어 금지** — '실패', '오류', '문제 발생' 대신 "다시 해볼까요?", "확인이 필요해요" 등 사용

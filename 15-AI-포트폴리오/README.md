# 15. AI로 포트폴리오 만들어 내보내고 배포하기 (실습 ⑥)

AI 도구로 포트폴리오 한 페이지를 만들고, 결과물을 HTML 파일로 내보내고,
코드를 읽고 직접 고친 뒤 Netlify에 배포합니다.

## 폴더 구성

| 파일 | 쓰는 때 | 내용 |
|---|---|---|
| prompt.md | Day 3 · 1~2단계 | 프롬프트 틀과 방법 A · B · C 별 내보내기 순서 |
| example/ | 막힐 때 참고 | AI에게 받은 결과물 예시 (index.html · style.css) |
| 수정-미션.md | Day 4 | 코드에서 직접 고칠 곳 목록과 기록표 |

## 무료로 파일을 받을 수 있는 세 가지 방법

| 방법 | 받는 것 | 알아 둘 것 |
|---|---|---|
| A. 채팅 AI (ChatGPT · Claude · Gemini 무료 버전) | index.html · style.css | 배운 코드 형태 그대로 나옵니다. 무료 버전은 대화 횟수 제한이 있습니다. |
| B. Claude Design | 단독 HTML 파일 | Free 플랜부터 됩니다. 사용량이 Claude 전체 한도에 합산됩니다. |
| C. Google Stitch | 화면별 HTML · CSS 코드 | Google 계정이면 됩니다. class가 Tailwind 방식일 수 있습니다. |

Framer · Figma Sites는 HTML 내보내기가 없고, Lovable · Manus · Figma Make는 받은 코드를
빌드해야 해서 폴더를 그대로 Netlify에 올릴 수 없습니다. (2026-11 기준, 수업 전 다시 확인)

## 요구사항

1. AI 도구로 포트폴리오 한 페이지 만들기 (섹션 4개: 소개 · 작업 · about · 연락처)
2. 결과물을 HTML 파일로 내보내 portfolio 폴더에 index.html 로 저장
3. 코드에서 3곳 이상 직접 고치기 (수정-미션.md)
4. Netlify에 배포하고 주소 제출

## example 폴더에 대해

example 은 방법 A의 프롬프트(prompt.md)로 받은 결과물을 정리한 예시입니다.
- header · nav · main · section · footer, Flex, Grid 등 이번 주에 배운 것으로만 되어 있습니다.
- 375px(모바일) · 768px · 1280px 에서 가로로 넘치지 않는 것을 확인했습니다.
- 이미지는 placehold.co 자리 표시 이미지입니다. 내 이미지로 바꿔 쓰세요.

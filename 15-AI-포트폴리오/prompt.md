# 프롬프트 틀

네 가지를 채웁니다: 목적 · 구조 · 톤 · 제약. [ ] 안을 내 내용으로 바꾸세요.

```
[이름]의 포트폴리오 웹사이트를 한 페이지로 만들어 줘.

목적: [채용 담당자]에게 [UX 작업 3개]를 보여 주는 사이트야.

구조 (위에서 아래 순서)
1. 헤더: 왼쪽에 이름, 오른쪽에 메뉴 (작업 · 소개 · 연락처)
2. 소개: 큰 제목 한 줄, 설명 두 줄
3. 작업: 카드 3개 (이미지 · 제목 · 한 줄 설명)
   - [작업 1 제목]: [한 줄 설명]
   - [작업 2 제목]: [한 줄 설명]
   - [작업 3 제목]: [한 줄 설명]
4. about: 프로필 사진과 소개 글
   - [자기소개 세 문장]
5. 연락처: 이메일 [주소], 링크 [링크드인 · 노션 등]

톤: [흰 배경, 보라색 포인트, 차분하고 여백이 넉넉하게]

제약
- 1컬럼 레이아웃, 본문 폭은 최대 960px
- 애니메이션은 넣지 마
- 이미지는 https://placehold.co 자리 표시 이미지로 넣어 줘
```

## 방법 A — 채팅 AI (ChatGPT · Claude · Gemini)

위 프롬프트 맨 아래에 이 세 줄을 더합니다.

```
- index.html 과 style.css 두 파일로 나눠 줘
- HTML과 CSS만 써 줘. 프레임워크와 JavaScript는 쓰지 마
- header · nav · main · section · footer 태그를 쓰고, 정렬은 Flex로 해 줘
```

1. 답으로 온 코드 블록 두 개를 각각 복사합니다.
2. VS Code에서 portfolio 폴더를 만들고 index.html · style.css 를 만들어 붙여 넣습니다.
3. 저장하고 index.html 을 더블클릭해 확인합니다.

고칠 때는 한 번에 한 가지만 요청합니다. 예) "작업 카드 사이 간격을 조금 넓혀 줘. style.css 전체를 다시 줘."

## 방법 B — Claude Design

1. Claude에서 위 프롬프트로 디자인을 요청합니다.
2. 큰 변경은 채팅으로, 일부만 고칠 때는 그 부분에 코멘트로, 위치와 크기는 캔버스에서 고칩니다.
3. 오른쪽 위 Export 에서 standalone HTML 을 골라 내려받습니다.
4. 받은 파일을 portfolio 폴더에 넣고 이름을 index.html 로 바꿉니다.

사용량이 Claude 전체 한도에 합산됩니다. 한도에 걸리면 방법 A로 바꿉니다.

## 방법 C — Google Stitch

1. stitch.withgoogle.com 에서 Web 을 고르고 위 프롬프트를 넣습니다.
2. 마음에 드는 화면을 고르고, 필요하면 다시 요청합니다.
3. 화면을 선택하고 Code 탭에서 HTML 을 복사합니다.
4. VS Code에서 portfolio 폴더에 index.html 을 만들어 붙여 넣고 저장합니다.

class 이름이 `flex justify-between items-center` 처럼 나오면 Tailwind 방식입니다.
`flex` = display: flex, `justify-between` = justify-content: space-between,
`items-center` = align-items: center 로 읽으면 됩니다.

## 공통 — 배포

1. portfolio 폴더 맨 위에 index.html 이 있는지 확인합니다.
2. 더블클릭으로 열어 깨진 곳이 없는지 봅니다.
3. Netlify에 폴더째 올립니다.
4. 무료 플랜은 한 달 배포 20회까지입니다. 내 컴퓨터에서 먼저 확인하고 올립니다.

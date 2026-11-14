# 파트4 [개발 프로세스 이해와 웹 퍼블리싱] — 실습용 예시 파일 모음

대본 기준으로 코드 예시/실습을 전부 실제 파일로 만들었습니다.   
폴더명 앞자리 숫자가 대본에서 등장하는 순서와 대응합니다. 각 폴더는 아래 둘 중 하나의 구성입니다.

- **practice / answer**: 학생이 직접 채워볼 실습용 파일 + 완성된 정답 파일
- **demo**: 실습이 아니라 강사가 라이브로 값을 바꿔가며 보여주는 시연용 파일 (정답이 따로 없음)


| 폴더                   | 대응 페이지    | 구성              | 내용                                                  |
| -------------------- | --------- | --------------- | --------------------------------------------------- |
| 01-개발환경-첫배포          | p.35      | practice/answer | Netlify에 처음 배포해보는 "안녕하세요" 페이지                       |
| 02-html-css-js-3단계데모 | p.40~42   | demo (3단계)      | HTML만 → HTML+CSS → HTML+CSS+JS 버튼 예제                |
| 03-css선택자-id-class실습 | p.52~53   | practice/answer | class로 글자색 바꾸기                                      |
| 04-html태그-종합데모       | p.62~74   | demo (1파일)      | 링크·제목·리스트·표·이미지·iframe·폼·div/span·시맨틱 태그 종합         |
| 05-html-자기소개           | 실습 ③     | practice/answer | header/nav/main/footer로 자기소개 (CSS 없음)               |
| 06-css속성-자기소개꾸미기     | 실습 ④     | practice/answer | 05 결과물에 폰트·색상·여백 CSS 적용 (practice = link·class 없는 상태 + 빈칸 CSS) |
| 07-박스모델-데모           | p.91~94   | demo            | padding 값 개수, margin auto, box-sizing 비교            |
| 08-배치방식-position-데모  | p.100~107 | demo            | block/inline/inline-block, position 5종              |
| 09-flex-정렬값-데모       | p.110     | demo            | justify-content 5종, align-items 4종, wrap, gap, grow |
| 10-flex-세로정렬-실습      | p.124~126 | practice/answer | 이미지+텍스트 Flex 세로 정렬                                  |
| 11-grid-데모           | p.119~123 | demo            | 컬럼/로우 나누기, fr, repeat, minmax, 배치, grid-area        |
| 12-javascript-AOS-실습 | p.129~132 | practice/answer | AOS 라이브러리로 스크롤 애니메이션 적용                             |
| 13-다중페이지-연결          | 신규 삽입분    | practice/answer | index/about/contact 페이지 연결 + CSS 공유                 |
| 14-최종포트폴리오-Cathy예시   | 실습 ⑥     | practice/answer/answer-4pages | practice=슬라이드 뼈대와 같은 시작 파일, answer=Cathy Kim 예시 원본(결과물 예시용), answer-4pages=패턴 1·2·3을 쓴 4페이지 완성 예시 |
| 15-AI-포트폴리오             | 실습 ⑥     | prompt/example  | AI로 만들어 내보내고 고쳐서 배포. prompt.md(방법 A·B·C) · example(결과물 예시) · 수정-미션.md |




## 사용 팁

- 모든 HTML 파일은 `index.html`(또는 폴더 내 지정 파일)을 브라우저로 더블클릭하면 바로 열립니다. 별도 서버 설정이 필요 없습니다.
- practice 폴더 파일들은 실제로 브라우저에서 열어도 "미완성" 상태로 보이는 게 정상입니다 (CSS 비어있음, 콘텐츠 비어있음 등).
- 이미지가 필요한 곳은 placehold.co(무료 플레이스홀더 이미지 서비스)를 썼습니다. 인터넷 연결이 필요합니다.


## 2026-11 수정 내역 (PD12)

- 폴더 이름을 Windows에서도 한글이 풀리지 않는 형태(NFC)로 다시 저장하고 macOS 부속 파일(__MACOSX, .DS_Store)을 뺐습니다.
- 모든 HTML에 viewport 메타 태그를 넣었습니다. (없으면 실제 휴대폰에서 축소되어 보입니다)
- 05 practice: 슬라이드와 같게 section · id 를 넣고 `href="#about"` 링크 설명을 주석으로 추가했습니다.
- 06 practice: 슬라이드 진행 순서(link 연결 → class 붙이기 → 빈칸 채우기)와 맞췄습니다. 내용은 answer와 같습니다.
- 06 answer: 웹 폰트 link(Noto Sans KR)를 실제로 넣었고, nav는 아직 배우지 않은 Flex 대신 text-align · margin 으로 바꿨습니다.
- 14 practice: 슬라이드 "2단계 뼈대"와 같은 구조(header > 로고 + nav, main, footer)로 바꾸고 class="header" · class="main" 을 미리 붙였습니다.
- 14 answer(Cathy 예시): `padding: 186px` → `padding: 186px 16px`. 넓은 화면에서는 전과 같고 모바일에서 본문 폭이 유지됩니다.
- 14 answer-4pages: 새로 추가한 4페이지 완성 예시입니다.
- 15-AI-포트폴리오: 실습 ⑥을 "AI로 생성 → 내보내기 → 읽고 고치기 → 배포"로 바꾸면서 추가했습니다. 14번(손코딩 4페이지)은 부록 · 심화용으로 남겼습니다.

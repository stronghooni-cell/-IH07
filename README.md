# 강성훈 자기소개 페이지

오즈코딩스쿨에서 배운 HTML·CSS·Bootstrap을 연결해 만든 자기소개 사이트입니다.
AI의 도움으로 기본 틀을 준비했습니다. 직접 수정하고 이해한 부분을 늘려가는 중입니다.

## 파일

```text
profile-portfolio/
  index.html
  style.css
  assets/
    profile.svg
  README.md
  .gitignore
```

`index.html`을 브라우저에서 열면 됩니다. Bootstrap과 아이콘은 CDN을 사용하므로 인터넷 연결이 필요합니다.

## 배운 기능을 사용한 곳

| 배운 내용 | 적용한 곳 |
|---|---|
| HTML 뼈대·제목·문단·목록 | 전체 문서와 자기소개·기술 카드 |
| 시맨틱 태그 | header·nav·main·section·article·aside·footer |
| 링크·내부 이동 | 상단 메뉴·본문 바로가기·맨 위로·GitHub 링크 |
| 이미지·대체 텍스트·상대 경로 | assets/profile.svg와 alt |
| 표·표 제목·제목 셀 | 학습 기록의 table·caption·th·scope |
| form·action·method·name | 의견을 GitHub의 작성 화면으로 넘기는 GET 폼 |
| label·input·textarea·button | 제목·내용·공개 확인·지우기 버튼 |
| required·pattern·maxlength | 필수 입력, 제목 공백 검사와 길이 제한 |
| checkbox | 공개되는 글인지 확인하는 체크박스 |
| radio·select·email·readonly·disabled | 연락처의 '배운 폼 요소 살펴보기' 모달. 선택·형식 오류 표시·초기화 연습 |
| fieldset·legend | 의견 입력 항목을 하나로 묶기 |
| 외부 CSS·선택자·캐스케이딩 | Bootstrap 다음에 style.css를 연결하고 내 스타일 적용 |
| 박스 모델·border-box | 카드 여백·테두리; Bootstrap Reboot의 border-box |
| Flexbox·gap·flex-wrap | 소개 영역·프로필 태그·버튼·푸터 |
| CSS Grid | 기술 카드 1열·2열·3열 배치 |
| relative·absolute·fixed·sticky | 프로필 배지·맨 위로 링크·상단 메뉴 |
| viewport·rem·max-width·미디어 쿼리 | 화면 폭별 배치, 최대 1080px 컨테이너 |
| max-width·height:auto | 프로필 이미지 크기 조절 |
| hover·focus·display | 카드 이동·키보드 포커스·펼쳐지는 메뉴 |
| CSS 변수·var·다크 모드 | 공통 색상과 기기의 어두운 화면 설정 |
| box-shadow·transition·transform | 카드 그림자와 마우스를 올렸을 때 이동 |
| Bootstrap CDN·bundle | 상단 스타일과 하단 script |
| container·row·col | 소개 7:5, 연락처 8:4, 작은 화면에서 세로 배치 |
| Button·Card·Form·Navbar·Modal | 버튼·기술 카드·연락처·접히는 메뉴·제작 이야기 |
| Utility·반응형 display·Icons | 여백·크기·d-none d-md-inline·아이콘 |

추가 폼 모달은 입력 요소를 조작해보는 연습용입니다. 입력한 내용은 저장·전송하지 않습니다. 실제 의견은 연락처의 GitHub 연결 폼을 사용합니다. 로그인·회원가입·메일 발송·자료 저장 기능은 구현하지 않았습니다.
Git 명령·브랜치·PR·개발자 도구·Live Share·AI 활용·MVP 등의 항목은 작업 방법이며, 화면 기능과 구분합니다. `.gitignore`와 이 README도 학습 범위에 맞춰 포함했습니다.

## 직접 바꿔볼 세 곳

1. index.html의 지원 동기 문장을 본인 말투로 고칩니다.
2. style.css의 `--accent-color`를 바꿔 색상 변화를 봅니다.
3. `.section-block`의 padding이나 `.hero-title`의 font-size를 바꿔 봅니다.

## 업로드 전에 확인

- 메뉴를 눌렀을 때 해당 영역으로 이동하는지
- 좁은 화면에서 메뉴 버튼을 누르면 메뉴가 펼쳐지는지
- 기술 카드가 모바일 1열, 768px 이상 2열, 992px 이상 3열인지
- '페이지 제작 이야기' 모달의 열기·닫기, Esc 키 동작
- 기기 설정을 다크 모드로 바꿨을 때 글자가 읽히는지
- 빈 의견 폼은 진행되지 않는지, '입력 지우기'가 동작하는지
- 의견을 작성하면 GitHub 새 글 화면으로 넘어가는지(등록은 직접 진행)

로컬 HTML과 CSS 연결·식별자·상대 경로·레이아웃 규칙을 정적으로 확인했습니다. Bootstrap CSS와 bundle의 다운로드 및 무결성 값, 아이콘 CSS의 다운로드도 확인했습니다.
현재 작업 환경에서 브라우저가 로컬 미리보기에 연결되지 않아 실제 화면과 메뉴·모달의 클릭 동작은 확인하지 못했습니다. 업로드 전 위 항목을 직접 확인해주세요.

## 기존 저장소에 최종본 올리기

기존에 GitHub와 연결해 둔 폴더에 이 폴더의 파일을 복사합니다. `assets` 폴더도 함께 넣습니다. 기존 `.git` 폴더는 유지합니다.

```powershell
git status
git add index.html style.css assets/profile.svg README.md .gitignore
git diff --cached
git commit -m "feat: 자기소개 사이트에 배운 기능 적용"
git push
```

기존의 같은 파일을 교체하고 변경 내용을 확인하는 순서입니다. `git init`이나 remote 연결을 반복할 필요는 없습니다.
GitHub Pages가 main / root로 설정되어 있다면 push 이후 자동 배포됩니다.
파일 묶음을 내려받는 것만으로는 원격 저장소에 반영되지 않습니다. 반영된 변경은 GitHub 커밋 기록에서 확인합니다.

## 참고

- [Bootstrap 5.3 시작하기](https://getbootstrap.com/docs/5.3/getting-started/introduction/)
- [Bootstrap Modal](https://getbootstrap.com/docs/5.3/components/modal/)
- [Bootstrap Icons](https://icons.getbootstrap.com/)
- 저장소: https://github.com/stronghooni-cell/-IH07

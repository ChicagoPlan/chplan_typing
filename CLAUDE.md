# chplan_typing — CLAUDE.md

초보자용 타자연습 웹페이지(자리·단어·문장 연습, 한국어/English). 운영 주소: https://type.chicagoplan.com

## 핵심 규칙 (개발·배포 시 항상 지킨다)
1. 코드는 이 GitHub 저장소(ChicagoPlan/chplan_typing)에 두고, 배포는 GitHub와 Cloudflare Pages의 Git 연동으로만 한다. main 브랜치 = 운영 주소.
2. 직접 업로드(Direct Upload), 파일 끌어다 놓기 배포는 쓰지 않는다.
3. 비밀번호, 키, 토큰은 저장소에 넣지 않는다.
4. 폰트는 저장소 fonts/ 의 나눔스퀘어네오(woff, 400/700)만 쓴다. 외부 CDN 링크 금지.
5. 구조: 빌드 없는 정적 페이지. index.html 한 파일 + fonts/. 빌드 명령 없음, 출력 폴더 루트(/).
6. 외부에 영향을 주는 행위(DNS 변경, 메일, 결제)는 건마다 보스 확인.

## 이름 (변경 불가 항목 포함)
- GitHub 저장소: ChicagoPlan/chplan_typing (공개)
- Cloudflare Pages 프로젝트: chplan-typing (주소 chplan-typing.pages.dev, 변경 불가)
- 사용자 지정 도메인: type.chicagoplan.com

## Drive 규칙 문서 위치 (먼저 읽는다)
- 공통 개발 규칙: 내 드라이브 > [CLAUDE] > __[Common] 공통참조자료 > __개발플랫폼_연동규칙 > 001_공통_개발인프라규칙_GitHub-Supabase-Cloudflare (최신 리비전)
- 운영 정책 마스터: 내 드라이브 > [CLAUDE] > __[Common] 공통참조자료 > Claude운영정책_Rev### (최신 리비전)
- 프로젝트 폴더(인수인계, INDEX): 내 드라이브 > [CLAUDE] > __[Chplan] 타자연습 (000_INDEX, 004_인수인계 최신 리비전)

## 작업 순서
새 브랜치에서 수정 → 미리보기 확인 → main에 병합 → 푸시 → 자동 배포. 소스 변경 후에는 Drive 003_결과물에 새 리비전 파일을 남기고 INDEX를 갱신한다.

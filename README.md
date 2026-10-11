# Sall Dashboard 공개 홈페이지

GitHub Pages에서 제공하는 앱 소개와 개인정보처리방침입니다.

- 현재 공개 홈페이지: https://sall-project.github.io/sall-dashboard-site/
- 현재 공개 개인정보처리방침: https://sall-project.github.io/sall-dashboard-site/privacy.html
- 연결할 도메인: https://dashboard.econsurge.com/
- 문의: keinpark1@gmail.com

## 구성

`index.html`, `privacy.html`, `styles.css`, `favicon.svg`만으로 동작합니다. 빌드, JavaScript, 데이터베이스, 로그인, 런타임 패키지가 필요하지 않습니다. `.nojekyll`은 GitHub Pages의 정적 파일 제공을 설정합니다.

## 배포

GitHub 저장소의 Settings → Pages에서 `main` 브랜치의 `/ (root)`를 게시 대상으로 선택합니다. DNS와 도메인 소유권을 확인한 뒤 Custom domain에 `dashboard.econsurge.com`을 설정하고 HTTPS를 활성화합니다.

Cloudflare에는 다음 레코드를 추가합니다. 기존 블로그 DNS 레코드는 수정하지 않습니다.

| 항목   | 값                     |
| ------ | ---------------------- |
| 유형   | CNAME                  |
| 이름   | dashboard              |
| 대상   | sall-project.github.io |
| 프록시 | DNS only               |
| TTL    | Auto                   |

`econsurge.com`의 Search Console 도메인 소유권 인증은 2026년 10월 11일 `keinpark1@gmail.com` 계정으로 완료했습니다. Google 브랜드 인증에는 도메인 연결이 완료된 후 `https://dashboard.econsurge.com/`, `https://dashboard.econsurge.com/privacy.html`과 승인된 도메인 `econsurge.com`을 등록합니다.

## 수정

페이지나 CSS를 수정한 뒤 `main`에 반영하면 다시 배포됩니다. 데이터 처리 방식이 바뀌면 개인정보처리방침의 내용과 적용일을 함께 갱신합니다. 공개 저장소에 토큰, 환경 설정, 로컬 데이터 또는 앱 백엔드 소스를 넣지 않습니다.

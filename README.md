# Sall Dashboard 공개 홈페이지

GitHub Pages에서 제공하는 앱 소개와 개인정보처리방침입니다.

- 홈페이지: https://dashboard.econsurge.com/
- 개인정보처리방침: https://dashboard.econsurge.com/privacy.html
- 공개 저장소: https://github.com/sall-project/sall-dashboard-site
- 문의: keinpark1@gmail.com

## 구성

`index.html`, `privacy.html`, `styles.css`, `favicon.svg`만으로 동작합니다. 빌드, JavaScript, 데이터베이스, 로그인, 런타임 패키지가 필요하지 않습니다. `.nojekyll`은 GitHub Pages의 정적 파일 제공을 설정하고, `CNAME`은 사용자 지정 도메인을 유지합니다.

## 배포

GitHub 저장소의 Settings → Pages에서 `main` 브랜치의 `/ (root)`가 게시 대상으로 설정되어 있습니다. Custom domain은 `dashboard.econsurge.com`입니다. HTTPS 인증서가 발급되어 Enforce HTTPS를 활성화했습니다. HTTP 요청은 HTTPS로 자동 전환됩니다.

Cloudflare에 다음 레코드가 설정되어 있습니다.

| 항목   | 값                     |
| ------ | ---------------------- |
| 유형   | CNAME                  |
| 이름   | dashboard              |
| 대상   | sall-project.github.io |
| 프록시 | DNS only               |
| TTL    | Auto                   |

`econsurge.com`의 Search Console 도메인 소유권 인증은 2026년 10월 11일 `keinpark1@gmail.com` 계정으로 완료했습니다. Google Cloud의 `sall-dashboard` 프로젝트 브랜드 설정에는 위 홈페이지와 개인정보처리방침 링크, 승인된 도메인 `econsurge.com`을 등록했습니다. Google 브랜드 인증과 게시를 완료했습니다. Google Ads API의 Basic Access 승인은 별도 절차입니다.

## 수정

페이지나 CSS를 수정한 뒤 `main`에 반영하면 다시 배포됩니다. 데이터 처리 방식이 바뀌면 개인정보처리방침의 내용과 적용일을 함께 갱신합니다. 공개 저장소에 토큰, 환경 설정, 로컬 데이터 또는 앱 백엔드 소스를 넣지 않습니다.

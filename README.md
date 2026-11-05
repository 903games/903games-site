# 903games.com 사이트

## 구성

| 주소 | 파일 | 용도 |
| --- | --- | --- |
| 903games.com | index.html | 스튜디오 소개, 게임 2개, 연락처 |
| 903games.com/privacy/ | privacy/index.html | 이누다치 개인정보처리방침 (플레이 스토어 등록에 필요) |
| 903games.com/probability/ | probability/index.html | 이누다치 확률 정보 |
| 903games.com/links/ | links/index.html | SNS 프로필에 거는 링크 모음 |
| 903games.com/inu/ | inu/index.html | 짧은 링크 → 플레이스토어 (출시 후 주소 교체) |
| 903games.com/dino/ | dino/index.html | 짧은 링크 → 스팀 상점 (공개 후 주소 교체) |
| 903games.com/app-ads.txt | app-ads.txt | AdMob 인증 파일 (AdMob에서 받은 줄 붙여넣기) |

노란 바탕 `[대괄호]` 부분이 채워야 할 곳입니다. 공개 전에 전부 지우세요.
개인정보처리방침은 초안입니다. 실제로 쓰는 SDK(광고·분석·저장)에 맞게 고치고, 가능하면 세무사·전문가에게 한 번 확인받으세요.

## 무료로 올리는 방법 (GitHub Pages)

1. GitHub에서 새 공개 저장소를 만든다 (예: `903games-site`).
2. 이 폴더의 파일을 전부 저장소 맨 위에 올린다 (Add file → Upload files).
3. 저장소 Settings → Pages → Source를 `main` 브랜치 `/ (root)`로 지정.
4. 같은 화면 Custom domain에 `903games.com` 입력 (CNAME 파일이 이미 들어 있음).
5. 도메인을 산 곳(구글 워크스페이스 가입 때 구매한 곳)의 DNS 설정에서:
   - A 레코드 4개, 호스트 `@`: `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - CNAME 레코드, 호스트 `www`: `[GitHub 아이디].github.io`
   - **MX, TXT 레코드는 건드리지 않는다** — 워크스페이스 메일이 여기에 걸려 있다.
6. 몇 분~몇 시간 뒤 Pages 화면에서 `Enforce HTTPS`를 켠다.

## 출시 전에 할 일

- 플레이 콘솔 스토어 등록정보의 연락처 웹사이트에 `https://903games.com` 입력
- 개인정보처리방침 URL에 `https://903games.com/privacy/` 입력
- AdMob app-ads.txt 줄을 붙여넣고 배포 → 24시간 안에 AdMob에서 인증 확인
- 출시 후 `inu/index.html`, 상점 공개 후 `dino/index.html`의 이동 주소 교체

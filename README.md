# hack-pm-dist

해킹 도메인 전용 앱 **hack-pm** 의 공개 배포 저장소. 소스는 private (`pTek0/hack-pm`).

## 설치
최신 APK 직링크:
https://github.com/pTek0/hack-pm-dist/releases/latest/download/hack-pm.apk

- 앱이 실행할 때 `releases/latest` 를 조회해 새 버전이면 알려주고 자동으로 내려받는다(원터치 설치).
- CI 가 **고정 키로 재서명**하므로 매 빌드 서명이 같아 **덮어 업데이트**가 된다.
- 패키지 ID 는 `dev.ptek.hackpm` — PM 앱(pm-mobile)과 별개로 설치된다.

## data/
| 파일 | 내용 |
|---|---|
| `changelog.json` | 버전별 패치노트(앱 설정 > 패치노트가 읽는다). 소스는 hack-pm 저장소의 `CHANGELOG.md`. |

진척률(`progress.json`) · 알림(`notifications.json`) · 호스트(`hosts.json`)는 PC 수집기가
`pTek0/pm-mobile-dist` 에 발행하며, hack-pm 은 그쪽을 그대로 읽는다(수집기 이원화 없음).

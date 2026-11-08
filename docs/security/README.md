# 보안 리포트 인덱스

최신 리포트: [2026-11-09](2026-11-09.md) · 이전: [2026-11-08](2026-11-08.md), [2026-11-07](2026-11-07.md), [2026-11-06](2026-11-06.md), [2026-11-05](2026-11-05.md), [2026-11-04](2026-11-04.md)

| ID | 최초 발견일 | 심각도 | 상태 | 요약 |
|---|---|---|---|---|
| F-01 | 2026-11-04 | Med | 수정(브랜치) | importmap `integrity`로 CDN 모듈 4개 해시 고정. Chromium에서 변조 차단 확인. Safari·Firefox 지원 여부 미확인(미지원 시 무시되고 정상 동작) |
| F-02 | 2026-11-04 | Med | 수정(브랜치) | CSP 메타 추가(`connect-src 'self' blob: data:`로 외부 전송 차단). 인라인 스크립트 때문에 `unsafe-inline` 유지 |
| F-05 | 2026-11-04 | Med | 부분 수정 | 20GB·8K·3시간 상한 추가. HEVC WASM의 Worker 이전은 미해결 |
| F-09 | 2026-11-05 | Med | 수정(브랜치) | mediabunny·prores 1.65.2로 업그레이드, integrity 해시 갱신 |
| F-10 | 2026-11-06 | Info | 확인 필요 | Safari의 importmap integrity 관련 WebKit 버그. PR #1 머지 전 실제 Safari 확인 |
| F-11 | 2026-11-09 | Low | 주시 | libav-hevc 내장 FFmpeg(6.x 추정)가 2026-09 이후 갱신 안 됨 |
| F-03 | 2026-11-04 | Low | 미해결 | Google Fonts 프라이버시 |
| F-04 | 2026-11-04 | Low | 미해결 | 로컬 모드·테스트 훅이 공개 빌드에 존재 |
| F-06 | 2026-11-04 | Low | 수정(브랜치) | `<meta name="referrer" content="no-referrer">` |
| F-07 | 2026-11-04 | Low | 미해결(수용 가능) | 클릭재킹 헤더 설정 불가 |
| F-08 | 2026-11-04 | Info | 종결 | setStatus textContent 확인(XSS 경로 없음) |

> 2026-11-04 수정분은 `ccr-7f9d7924-5dyc1m` 브랜치에 있음. main에 합쳐야 배포됨.

<h2>
  Jaeseong Oh (rojae)
  <a href="https://hits.sh/github.com/rojae">
    <img alt="Hits" src="https://hits.sh/github.com/rojae.svg?view=today-total&logo=github" align="right"/>
  </a>
</h2>

**커머스와 결제 분야에서 6년 이상 개발·운영한 Java/Spring 백엔드 개발자.**

회원·인증·외부 제휴 연동을 만들며 동시 갱신, 부분 실패, 운영자의 후속 처리를 다뤄 왔습니다. 어떤 데이터를 함께 바꿔야 하는지, 실패했을 때 무엇을 보존하고 다시 처리할지를 정하며 개발합니다.

<a href="https://rojae.kr"><img src="https://img.shields.io/badge/rojae.kr-2f5bd8?style=flat-square&logo=safari&logoColor=white" alt="Website"/></a>
<a href="https://rojae.kr/resume.pdf"><img src="https://img.shields.io/badge/Resume%20PDF-000000?style=flat-square&logo=adobeacrobatreader&logoColor=white" alt="Resume PDF"/></a>
<a href="https://rojae.github.io"><img src="https://img.shields.io/badge/Blog-171717?style=flat-square&logo=jekyll&logoColor=white" alt="Blog"/></a>
<a href="https://medium.com/@jaethon96"><img src="https://img.shields.io/badge/Medium-171717?style=flat-square&logo=medium" alt="Medium"/></a>

## Work

- [외부 파트너 제휴 연동](https://rojae.kr/work/affiliate.html) — 인증 후 동의 항목의 실패가 이미 완료된 인증·다른 동의를 되돌리지 않도록 트랜잭션을 분리했습니다. 일배치 첫 묶음이 동시에 도착할 때 마스터 행 생성 충돌이 본 처리를 실패시키지 않도록 생성만 별도 트랜잭션으로 격리했습니다. 중복 검사·누적 갱신은 같은 배치의 행 잠금 안에서 처리했습니다. 백엔드 쿠폰 실패 건의 주기 재처리를 운영해 뒤늦게라도 고객이 이벤트 혜택을 받도록 했습니다.
- [통합인증](https://rojae.kr/work/auth.html) — 세 사이트의 다섯 인증 유형을 통합하고, 장애 횟수의 동시 갱신은 Redis Lua 원자 연산으로 처리했습니다. 상태 변경을 Pub/Sub으로 Caffeine 캐시에 전파하고, 알림 누락은 RDB 원천의 주기 재동기화로 보완했습니다. 장애 인증사 자동 비활성화·비율 조정은 구현했으며, 정상화 후 원래 비율로 자동 복귀하는 기능은 설계 검토 단계로 남았습니다.
- [약관 관리](https://rojae.kr/work/terms.html) — 사이트별 약관 본문·버전·시행일과 화면별 구성을 분리했습니다. 시행일에 따른 노출은 자동화하고, 등록 오류를 수정할 수 있도록 버전 번호는 운영자가 관리하게 했습니다. 모델 설계·주요 구현과 공동 발표를 맡았습니다.
- [전자문서 유통](https://rojae.kr/work/edoc.html) — 2인 팀에서 서버 22대 환경의 인프라 설계와 API·관리자·배치를 맡았습니다. 라이선스 비용을 고려한 Galera 구성에서 DB 복제와 접속 경로를 분리하고, 재기동·인증서 갱신·순차 배포 절차를 인계했습니다. 인증 심사 준비·보완에 참여했고 서비스는 2차 심사에서 적합 판정을 받았습니다.
- [회원 공통 모듈](https://rojae.kr/work/platform.html) — 사이트별 중복 구현을 줄이는 구조를 팀과 설계하고 제휴·인증 모듈을 개발했습니다. [로그인 전환](https://rojae.kr/work/login.html)에서는 DB 연결 장애 분석과 Java/Spring 전환 설계에 참여했습니다.

## Open Source

| Project | | |
|---|---|---|
| [OpenFluxGate](https://github.com/OpenFluxGate/fluxgate) | 동시 요청의 제한 상태 확인·차감을 Redis Lua로 원자 처리. 앱 시계 차이는 Redis TIME으로 줄이고, EVALSHA와 동적 인자로 스크립트 본문의 반복 전송을 줄임. Spring Boot 스타터·[관리 어드민](https://github.com/OpenFluxGate/fluxgate-studio), 개인 OSS·사내 POC | ![Maven Central](https://img.shields.io/maven-central/v/io.github.openfluxgate/fluxgate-core?style=flat-square&label=maven) |
| [WAF 플랫폼](https://rojae.kr/work/waf.html) | Nginx + ModSecurity + OWASP CRS, 실시간 / 분석 트랙으로 나눈 로그 파이프라인 (외부 스터디 · 단독 구현) | Java · Go · TS |
| [Auth Server](https://github.com/rojae/auth-server-be) | Spring Authorization Server 기반 회원 · 인증 서비스 (현재 서비스 중단) | Java |
| [FluxMirror](https://github.com/OpenFluxGate/fluxmirror) | Claude Code · Gemini CLI · Qwen Code 활동 감사 도구 | Rust |
| [IssueLinker](https://plugins.jetbrains.com/plugin/30083-issuelinker) | 브랜치 이름의 이슈 키를 Jira · GitHub 이슈로 바로 여는 IntelliJ 플러그인 | Kotlin |
| [GitChan](https://github.com/gitchan-app/gitchan) | Live2D 마스코트가 붙은 GitHub 알림 앱 (Gitify 기반) | TypeScript |

### Contributions

- [OpenFeign/feign #2871](https://github.com/OpenFeign/feign/pull/2871) — `RetryableException`에 `retryAfter` 없는 생성자 추가 (Kotlin 오버로드 모호성 해소)
- [OpenFeign/feign #2874](https://github.com/OpenFeign/feign/pull/2874) — 어노테이션 파라미터 값 누락 시 힌트 메시지

## Writing

- [FluxGate의 Lua: 차감을 한 번에 묶고도 남는 실패 경계](https://rojae.github.io/posts/fluxgate-lua-atomicity-and-failure-boundaries/) — Lua·EVALSHA·규칙 변경 알림을 선택한 이유와 다중 제한·재시도의 범위
- [백엔드 설계의 경계: 실패를 어디까지 함께 책임질 것인가](https://rojae.github.io/posts/backend-design-decisions-and-operational-boundaries/) — 통합인증·제휴·전자문서에서 함께 처리할 상태와 따로 복구할 실패를 정한 경험
- [JVM DNS Caching Meets Connection Pools](https://rojae.github.io/posts/jvm-dns-caching-meets-connection-pools/) — IP 변경 뒤의 장애를 기존 HTTP 연결 재사용과 새 연결의 DNS 조회로 나눠 분석·재현하고 내부 공유 ([English](https://medium.com/@jaethon96/how-is-dns-managed-in-jvm-0b1cadd08ba2))
- [Spring Batch 실전 시리즈](https://rojae.github.io/posts/spring-batch-intro/) — 개념, 핵심 인터페이스, 발송 배치, 성능 최적화
- [서비스가 커질수록 필요한 설계 패턴](https://rojae.github.io/posts/design-pattern-intro/) — 메시징 시스템 예제로 보는 Factory · Strategy · Template Method · CoR
- [젊은 로재씨의 슬픔 — 우당탕탕 PL 데뷔기](https://rojae.github.io/posts/the-sorrows-of-young-rojae/)

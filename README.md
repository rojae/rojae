<h2>
  Jaeseong Oh (rojae)
  <a href="https://hits.sh/github.com/rojae">
    <img alt="Hits" src="https://hits.sh/github.com/rojae.svg?view=today-total&logo=github" align="right"/>
  </a>
</h2>

**6년 차 Java/Spring 서버 개발자.** 지금은 지마켓 Member Engineering에서 인증 · 제휴 연동 · 약관을 맡고 있습니다. 전자금융 PG와 커머스에서 회원 · 인증 · 외부 파트너 연동을 만들고 운영해 왔고, 기능이 동작하는 순간만큼 실패하고 회복하는 경계와 그 뒤의 운영을 중요하게 생각합니다.

<a href="https://rojae.kr"><img src="https://img.shields.io/badge/rojae.kr-2f5bd8?style=flat-square&logo=safari&logoColor=white" alt="Website"/></a>
<a href="https://drive.google.com/file/d/1BdjvsehWxIfhAOJmOlzCTRp8qkAu_Jo2/view?usp=sharing"><img src="https://img.shields.io/badge/Resume%20PDF-000000?style=flat-square&logo=googledrive&logoColor=white" alt="Resume PDF (Google Drive)"/></a>
<a href="https://rojae.github.io"><img src="https://img.shields.io/badge/Blog-171717?style=flat-square&logo=jekyll&logoColor=white" alt="Blog"/></a>
<a href="https://medium.com/@jaethon96"><img src="https://img.shields.io/badge/Medium-171717?style=flat-square&logo=medium" alt="Medium"/></a>

## Work



- [외부 파트너 제휴 연동 플랫폼](https://rojae.kr/work/affiliate.html) — 삼성카드 첫 적용, 양방향 동의 · 배치 정합 · 리워드 · 운영 어드민, 오픈 첫 달 동의 약 1만 명
- [통합인증 서비스](https://rojae.kr/work/auth.html) — 6가지 인증 유형과 인증업체 비율을 어드민에서 다루는 공통 인증, 월 인증 비용 약 1/3↓ · CS 90%↓
- [약관 관리 서비스](https://rojae.kr/work/terms.html) — 지마켓 · 옥션 · ESMPLUS 약관을 한 서비스로 통합, 약관 동의 서비스로 확장해 운영 중
- [전자문서 유통 서비스](https://rojae.kr/work/edoc.html) — 서버 22대 이중화 인프라부터 API · 관리자 · 배치까지, KISA 전자문서유통중계자 인증 심사 적합
- [회원 도메인 공통 모듈화](https://rojae.kr/work/platform.html) · [로그인 시스템 Java/Spring 전환](https://rojae.kr/work/login.html) · [WAF 플랫폼 (스터디)](https://rojae.kr/work/waf.html)

## Open Source

| Project | | |
|---|---|---|
| [OpenFluxGate](https://github.com/OpenFluxGate/fluxgate) | Redis 기반 분산 Rate Limiting 라이브러리 + Spring Boot 스타터 + [관리 어드민](https://github.com/OpenFluxGate/fluxgate-studio) | ![Maven Central](https://img.shields.io/maven-central/v/io.github.openfluxgate/fluxgate-core?style=flat-square&label=maven) |
| [WAF 플랫폼](https://rojae.kr/work/waf.html) | Nginx + ModSecurity + OWASP CRS, 실시간 / 분석 트랙으로 나눈 로그 파이프라인 (외부 스터디 · 단독 구현) | Java · Go · TS |
| [Auth Server](https://github.com/rojae/auth-server-be) | Spring Authorization Server 기반 회원 · 인증 서비스 (현재 서비스 중단) | Java |
| [FluxMirror](https://github.com/OpenFluxGate/fluxmirror) | Claude Code · Gemini CLI · Qwen Code 활동 감사 도구 | Rust |
| [IssueLinker](https://plugins.jetbrains.com/plugin/30083-issuelinker) | 브랜치 이름의 이슈 키를 Jira · GitHub 이슈로 바로 여는 IntelliJ 플러그인 | Kotlin |
| [GitChan](https://github.com/gitchan-app/gitchan) | Live2D 마스코트가 붙은 GitHub 알림 앱 (Gitify 기반) | TypeScript |

### Contributions

- [OpenFeign/feign #2871](https://github.com/OpenFeign/feign/pull/2871) — `RetryableException`에 `retryAfter` 없는 생성자 추가 (Kotlin 오버로드 모호성 해소)
- [OpenFeign/feign #2874](https://github.com/OpenFeign/feign/pull/2874) — 어노테이션 파라미터 값 누락 시 힌트 메시지

## Writing

- [JVM DNS Caching Meets Connection Pools](https://rojae.github.io/posts/jvm-dns-caching-meets-connection-pools/) — IP 변경 뒤의 프로덕션 장애를 JVM DNS 캐시 관점에서 ([English](https://medium.com/@jaethon96/how-is-dns-managed-in-jvm-0b1cadd08ba2))
- [Spring Batch 실전 시리즈](https://rojae.github.io/posts/spring-batch-intro/) — 개념, 핵심 인터페이스, 발송 배치, 성능 최적화
- [서비스가 커질수록 필요한 설계 패턴](https://rojae.github.io/posts/design-pattern-intro/) — 메시징 시스템 예제로 보는 Factory · Strategy · Template Method · CoR
- [젊은 로재씨의 슬픔 — 우당탕탕 PL 데뷔기](https://rojae.github.io/posts/the-sorrows-of-young-rojae/)

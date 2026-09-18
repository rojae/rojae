<h2>
  Jaeseong Oh (rojae)
  <a href="https://hits.sh/github.com/rojae">
    <img alt="Hits" src="https://hits.sh/github.com/rojae.svg?view=today-total&logo=github" align="right"/>
  </a>
</h2>

Server engineer. 회원 · 인증 · 외부 파트너 연동을 만듭니다. Java / Spring.

<a href="https://rojae.kr"><img src="https://img.shields.io/badge/rojae.kr-2f5bd8?style=flat-square&logo=safari&logoColor=white" alt="Website"/></a>
<a href="https://rojae.kr/resume.html"><img src="https://img.shields.io/badge/Resume-000000?style=flat-square&logo=readme&logoColor=white" alt="Resume"/></a>
<a href="https://rojae.github.io"><img src="https://img.shields.io/badge/Blog-171717?style=flat-square&logo=jekyll&logoColor=white" alt="Blog"/></a>
<a href="https://medium.com/@jaethon96"><img src="https://img.shields.io/badge/Medium-171717?style=flat-square&logo=medium" alt="Medium"/></a>

## Work

프로젝트별 상세 글은 **[rojae.kr](https://rojae.kr)** 에 있습니다.

- [외부 파트너 제휴 연동 플랫폼](https://rojae.kr/work/affiliate.html) — 양방향 동의 · 배치 정합 · 리워드 · 운영 어드민
- [통합인증 서비스](https://rojae.kr/work/auth.html) — 6가지 인증 유형과 인증업체 비율을 어드민에서 다루는 공통 인증
- [약관 관리 서비스](https://rojae.kr/work/terms.html) — 지마켓 · 옥션 · ESMPLUS 약관을 한 서비스로
- [회원 도메인 공통 모듈화](https://rojae.kr/work/platform.html) · [로그인 시스템 Java/Spring 전환](https://rojae.kr/work/login.html)

## Open Source

| Project | | |
|---|---|---|
| [OpenFluxGate](https://github.com/OpenFluxGate/fluxgate) | Redis 기반 분산 Rate Limiting 라이브러리 + Spring Boot 스타터 + [관리 어드민](https://github.com/OpenFluxGate/fluxgate-studio) | ![Maven Central](https://img.shields.io/maven-central/v/io.github.openfluxgate/fluxgate-core?style=flat-square&label=maven) |
| [WAF](https://github.com/rojae/waf) | Nginx + ModSecurity + OWASP CRS, 실시간 / 분석 트랙으로 나눈 로그 파이프라인 | Java · Go · TS |
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

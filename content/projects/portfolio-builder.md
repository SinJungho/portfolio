---
title: 포트폴리오 빌더
description: 편집·미리보기 서비스의 성능과 검증 환경을 개선한 개인 프로젝트
---

# 포트폴리오 빌더

[서비스 바로가기](https://portfolio-builder-woad.vercel.app) · [GitHub 저장소](https://github.com/SinJungho/portfolio-builder)

## 문제와 역할

에디터·미리보기·마케팅 화면을 개편하면서 렌더링 경로와 무거운 모달·폰트·Hero 애니메이션을 점검했습니다. 인증과 공통 API 오류 흐름까지 직접 구현·보완했습니다.

## 구현과 검증

- `useDeferredValue`·`useTransition`·`React.memo`를 적용해 렌더링 경로를 조정했습니다.
- GitHub OAuth와 JWT/Prisma 세션, 토큰 암호화·재인증 흐름을 구현했습니다.
- 공통 API 오류 응답·로그를 표준화하고 Redis 장애 응답·동기화 흐름을 보완했습니다.
- GitHub Actions·Lighthouse CI를 연결해 성능을 검증했습니다. 확인된 기준은 Lighthouse Performance 94점, LCP 3.1초입니다.
- Jest·React Testing Library 기준 49개 스위트, 158개 테스트 통과 결과를 확인했습니다.

## 근거

- [에디터·미리보기·마케팅 화면 개편](https://github.com/SinJungho/portfolio-builder/commit/34f04e5c72e95898aaa55bc11e73984bb9b6a5fd)
- [공통 API 오류 응답·로그 표준화](https://github.com/SinJungho/portfolio-builder/commit/9303cece8ed1967428bf32926d4869304cc6652a)
- [접근성 회귀 테스트](https://github.com/SinJungho/portfolio-builder/commit/7e840bf34c53bb4b6175824d88dfaf22300d64a5)

---
title: 포트폴리오 빌더
description: 편집·미리보기 서비스의 성능과 검증 환경을 개선한 개인 프로젝트
---

> 에디터·미리보기·마케팅 화면을 개편하고, 렌더링·인증·API 오류 흐름을 직접 검증한 개인 프로젝트입니다.

[서비스 바로가기](https://portfolio-builder-woad.vercel.app) · [GitHub 저장소](https://github.com/SinJungho/portfolio-builder)

## 프로젝트 한눈에 보기

| 항목        | 내용                                                      |
| ----------- | --------------------------------------------------------- |
| 범위        | 에디터·미리보기·마케팅 화면, 인증, 공통 API 오류 처리     |
| 성능 기준   | Lighthouse Performance 94점, LCP 3.1초                    |
| 테스트 기준 | Jest·React Testing Library 49개 스위트, 158개 테스트 통과 |
| 검증 자동화 | GitHub Actions, Lighthouse CI                             |

## 핵심 과제

화면 개편 과정에서 렌더링 경로와 무거운 모달·폰트·Hero 애니메이션을 점검하고, 인증과 공통 API 오류 흐름을 일관되게 처리했습니다.

## 구현 범위

- `useDeferredValue`·`useTransition`·`React.memo`를 적용해 렌더링 경로를 조정했습니다.
- GitHub OAuth와 JWT/Prisma 세션, 토큰 암호화·재인증 흐름을 구현했습니다.
- 공통 API 오류 응답·로그를 표준화하고 Redis 장애 응답·동기화 흐름을 보완했습니다.

## 검증 결과

| 기준        | 확인 결과                                                 |
| ----------- | --------------------------------------------------------- |
| 성능        | Lighthouse Performance 94점, LCP 3.1초                    |
| 회귀 테스트 | Jest·React Testing Library 49개 스위트, 158개 테스트 통과 |
| 자동화      | GitHub Actions·Lighthouse CI 연결                         |

## 근거

- [에디터·미리보기·마케팅 화면 개편](https://github.com/SinJungho/portfolio-builder/commit/34f04e5c72e95898aaa55bc11e73984bb9b6a5fd)
- [공통 API 오류 응답·로그 표준화](https://github.com/SinJungho/portfolio-builder/commit/9303cece8ed1967428bf32926d4869304cc6652a)
- [접근성 회귀 테스트](https://github.com/SinJungho/portfolio-builder/commit/7e840bf34c53bb4b6175824d88dfaf22300d64a5)

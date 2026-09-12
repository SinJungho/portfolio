---
title: PetGround 홈페이지·관리자 CMS
description: 사용자 홈페이지와 관리자 CMS의 입력 검증, 인증, 파일 업로드를 구현한 프로젝트
---

# PetGround 홈페이지·관리자 CMS

`2024.11–2025.02` · 프론트엔드 개발자

## 맡은 범위

- React·TypeScript·Vite로 사용자 홈페이지와 콘텐츠 관리용 관리자 페이지를 개발했습니다.
- 관리자 등록·수정 화면에 React Hook Form·Zod 기반 입력값·이미지 검증을 적용하고 로그인·로그아웃 및 토큰 만료 처리를 구현했습니다.
- S3 Presigned URL 업로드와 일반 API 인증 요청을 분리해 Axios interceptor와 업로드 요청의 헤더 충돌을 피하고 이미지 업로드 오류를 보완했습니다.
- 메인·회사 소개·제품 소개·소식·FAQ의 API·라우팅과 슬라이더·필터·페이지네이션·무한 스크롤을 구현했습니다.
- Google Translate API와 한·영 약관·개인정보 처리방침 화면을 구성했습니다.

## 근거 저장소

- [관리자 저장소](https://bitbucket.org/cyglobal/fompet-homepage-admin)
- [사용자 저장소](https://bitbucket.org/cyglobal/fompet-homepage-web)
- [Presigned URL 업로드 구현](https://bitbucket.org/cyglobal/fompet-homepage-admin/commits/9058eec)
- [사용자 페이지 API 연결](https://bitbucket.org/cyglobal/fompet-homepage-web/commits/2d2b9b3)

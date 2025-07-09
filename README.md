# Spring MVC를 이용한 인증 기능 구현 연습 (Spring-MVC-Authentication-Practice)

이 저장소는 Spring Security와 같은 프레임워크에 의존하지 않고, 순수 Spring MVC의 핵심 기능을 활용하여 인증(Authentication) 및 인가(Authorization)를 구현하는 방법을 연습하기 위한 프로젝트입니다.

## 프로젝트 개요

본 프로젝트는 Spring MVC의 `HandlerInterceptor`와 `HandlerMethodArgumentResolver`를 사용하여 로그인 상태를 확인하고, 컨트롤러에서 인증된 사용자 정보를 간편하게 주입받는 과정을 학습하는 것을 목표로 합니다.

## 주요 학습 목표

  - **세션(Session) 기반 로그인/로그아웃:** `HttpSession`을 이용한 기본적인 로그인 및 로그아웃 기능 구현
  - **인증 체크 인터셉터:** `HandlerInterceptor`를 사용하여 특정 경로에 접근하는 사용자의 인증 상태를 확인
  - **Argument Resolver를 이용한 사용자 정보 주입:** `@Login`과 같은 커스텀 애너테이션과 `HandlerMethodArgumentResolver`를 구현하여, 인증된 사용자 객체를 컨트롤러 메서드의 파라미터로 손쉽게 전달
  - **인증/인가 로직 분리:** MVC의 각 컴포넌트 역할을 명확히 이해하고, 인증/인가 관련 코드를 체계적으로 분리
  - **테스트 코드 작성:** 구현된 인증 기능에 대한 단위 테스트 및 통합 테스트 코드 작성

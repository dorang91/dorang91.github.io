---
layout: post
title: "알아두면 좋은 커밋 가이드라인 (Conventional Commits)"
categories: [dev]
---

# 알아두면 좋은 커밋 가이드라인 (Conventional Commits)

## 1. 형식

- `type`: 커밋 종류
- `scope`: 영향받는 범위 (선택)
- `subject`: 한 줄 요약 (현재형, 마침표 X)

---

## 2. 주요 type

- **feat**: 새로운 기능 추가
- **fix**: 버그 수정
- **docs**: 문서 수정
- **style**: 포맷팅, 세미콜론 누락 등 (코드 변화 없음)
- **refactor**: 리팩터링 (동작 변화 없음)
- **test**: 테스트 추가·수정
- **chore**: 빌드, 패키지 매니저, 설정 변경 등

---

## 3. 예시

```text
feat(post): 블로그 새 글 작성 기능 추가
fix(config): baseurl 잘못된 값 수정
docs(readme): 설치 방법 보강
style(post): 코드 블록 들여쓰기 수정
refactor(theme): 레이아웃 컴포넌트 단순화
test(api): 포스트 API 단위 테스트 추가
chore(deps): jekyll-sitemap 버전 업데이트
```

---

팀이 없더라도 **feat / fix / docs / chore** 네 가지부터 일관되게 사용하면 충분합니다.
scope는 선택 사항이라 `feat: 회원가입 기능 추가`처럼 생략해도 됩니다.  
subject는 항상 **현재 시제, 짧고 명확하게** 쓰는 것이 원칙입니다.

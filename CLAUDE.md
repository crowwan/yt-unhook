# yt-unhook

아이폰 Safari(m.youtube.com)에서 Shorts·추천·댓글 등 주의를 빼앗는 요소를 숨기는 유저스크립트. iOS Userscripts 앱으로 설치한다.

## 개발 규칙

개인 프로젝트 공용 규칙(`~/Works/personal/_playbook/PLAYBOOK.md`)을 따른다.

- 기획: `docs/prd.md`, `docs/specs/SPEC-*.md` — 스펙이 동작의 기준. 구현 중 동작이 바뀌면 스펙부터 고친다.
- 작업: GitHub Issues + 마일스톤 (Projects 보드 미사용). 이슈는 approved 스펙에서만 만든다 (`/spec-issues`).
- 브랜치 `<종류>/<이슈번호>-<이름>`, 커밋 `feat: 한글 메시지 (#12)`, PR 로만 머지 (squash).
- 테스트: 스펙 ID 를 테스트 묶음 이름에, AC 내용을 테스트 이름에 한글로.
- 릴리스: `/release v0.x`

## 현재 상태

- 마일스톤: v0.1
- 진행 중 스펙: (없음, `docs/prd.md` 작성 전)
- Projects 보드: 사용 안 함 (라벨·마일스톤만)

## 스택

- TypeScript → 단일 `dist/yt-unhook.user.js` 로 빌드 (빌드 도구는 첫 이슈에서 결정)
- 테스트: Vitest (+ jsdom)
- 실행 환경: iOS Safari + Userscripts 앱 (quoid/userscripts). `GM.registerMenuCommand`, `unsafeWindow` 없음 → 설정 UI는 페이지 안에 직접 그린다
- 대상 사이트: `m.youtube.com` (모바일 DOM, `ytm-*` 요소)

## 실행

```bash
# 빌드 / 테스트 / 실행 명령
```

## 폴더 구조

```
```

---
description: 스테이징된 변경사항으로 커밋 생성
allowed-tools: Bash(git diff:*), Bash(git commit:*), Bash(git status:*)
---

## 현재 변경사항
!`git diff --cached`

## 작업
1. 위 diff를 분석해서 변경 내용을 요약합니다.
2. Conventional Commits 형식(feat:, fix:, chore: 등)으로 커밋 메시지를 작성합니다.
3. `git commit -m "..."`으로 커밋을 실행합니다.
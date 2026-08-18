---
description: 테스트 실행 후 커밋 & 푸시 (배포)
allowed-tools: Bash(cd apps/api && python -m pytest:*), Bash(git:*)
---

아래 워크플로우를 순서대로 실행한다.

## 1. 테스트 실행
`cd apps/api && python -m pytest` 로 백엔드 테스트 전체를 실행한다.

## 2. 테스트 실패 시
실패 내용을 보고하고 **중단**한다. commit/push 하지 않는다.

## 3. 테스트 전체 통과 시
아래 순서로 실행한다:
1. `git add -A` - 변경된 파일 전체 스테이징
2. `git diff -- staged` 로 변경 내용을 분석하여 적절한 커밋 메시지를 자동 작성
3. `git coamit` - 작성한 메시지로 커밋
4. `git push origin <현재브랜치>` - 현재 브랜치에 푸시

## 4. 결과 요약
push 완료 후 결과를 요약 출력한다.
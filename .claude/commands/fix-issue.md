---
description: 지정한 GitHub 이슈 번호의 버그를 수정
argument-hint: [issue-number]
allowed-tools: Bash, Read, Edit, Grep
---

이슈 #$ARGUMENTS 를 수정합니다.

1. `gh issue view $ARGUMENTS`로 이슈 내용을 확인합니다.
2. 관련 코드를 찾아 원인을 분석합니다.
3. 수정 후 관련 테스트를 실행해 검증합니다.
4. 변경 요약을 알려줍니다.
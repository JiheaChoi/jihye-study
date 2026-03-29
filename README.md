# mail-router

항공사 해외지점 시스템 장애/오류 메일을 자동으로 요약해 담당자 Slack으로 라우팅하는 시스템.

## 설계 문서

[DESIGN.md](./DESIGN.md) 참조

## 기술 스택

- Python (polling service)
- Gmail API (`google-auth` + `googleapiclient`)
- GPT-4o-mini (메일 분류 + 요약)
- Slack Incoming Webhook
- SQLite (상태 관리 + 라우팅 테이블)

## 시작하기

> 현재 설계 단계. 구현 시작 전 [DESIGN.md](./DESIGN.md)의 **The Assignment** 섹션부터 실행할 것.

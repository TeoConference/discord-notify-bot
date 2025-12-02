# 🤖 Discord Notify Bot

워크플로우 조회하는 시점 기준 읽지 않은 이메일을 조회해 디스코드 알림을 보내는 워크플로우입니다.

> 10분마다 안 읽은 메일 조회 트리거는 2025 테오콘 CX 계정의 GAS(Google App Script)에서 확인할 수 있습니다 

## 워크플로우 실행 방법

해당 레포지토리 Actions 내의 좌측에서 Discord Notify Bot 선택 후 `Run workflow`로 수동 실행 할 수 있습니다

![img](https://private-user-images.githubusercontent.com/124546770/520497776-711de620-3eb3-49eb-97bd-c5c970a10dde.png?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NjQ2ODU5ODgsIm5iZiI6MTc2NDY4NTY4OCwicGF0aCI6Ii8xMjQ1NDY3NzAvNTIwNDk3Nzc2LTcxMWRlNjIwLTNlYjMtNDllYi05N2JkLWM1Yzk3MGExMGRkZS5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjUxMjAyJTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI1MTIwMlQxNDI4MDhaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT1hODZkOTNlOWNjYTFlYjk3YTA5MjlkOWFiMWQ5OWZhYjZjMDE3ZmVlOWM0MDI4M2I5OTkzYTdiZDQwZDkwMjM2JlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCJ9.jbdACd2F6QPIulBncKG5VWRAcXKv5lOO9TeuIr-ujiA)

## 기능

### index.js
- App Script 훅을 요청해 읽지않은 이메일을 가져옵니다.
- 디스코드에 보낼 메시지 템플릿을 만들어 출력합니다.

### GAS (Google App Script)
- 테오콘 CX 계정 내의 읽지 않은 메시지에 `문의`, `결제`, `협찬` 키워드가 있을 시 라벨링을 합니다.
- 읽지 않은 메일 배열을 출력합니다.

## 이메일 웹훅 워크플로우 수정 방법

테오콘 CX 계정의 Google App Script 내의 '디스코드 알림 봇' 프로젝트에서 워크플로우를 수정할 수 있습니다.

> 2025 CX 계정 : team.teoconf@gmail.com

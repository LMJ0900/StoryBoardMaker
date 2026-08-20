# 브랜치 워크플로우 규칙

모든 작업은 `main`에 직접 커밋하지 않고, 작업 단위 브랜치를 생성해 PR(리퀘스트)로 진행한다.

## 절차

1. 새로운 작업을 시작하기 전, `main`에서 작업 단위 브랜치를 생성한다.
2. 해당 브랜치에서 작업 및 커밋을 진행한다. (커밋 컨벤션은 [commit-convention.md](./commit-convention.md) 참고)
3. 작업이 끝나면 PR을 생성해 `main`으로 머지 요청한다.
4. 리뷰/머지가 끝나면 `main`은 항상 클린한 상태를 유지한다.

## 브랜치 이름 규칙

`{type}/{작업-내용}` 형식을 따른다.

| type | 설명 |
|---|---|
| `feature` | 기능 추가 |
| `fix` | 버그 수정 |
| `docs` | 문서 관련 작업 |
| `refactor` | 리팩터링 |
| `chore` | 패키지/설정 등 잡무성 작업 |

예: `feature/initial-project-setup`, `docs/add-project-rules`

## 예외: README 전용 브랜치

`README.md` 수정은 매번 새 브랜치를 만들지 않고, 항상 `docs/readme-updates` 브랜치 하나에 커밋해서 PR을 보낸다. README 변경 건이 생길 때마다 이 브랜치를 다시 checkout해서 이어서 작업한다.

## 참고

리퀘스트(요청) 완료 후 노션 문서화는 [notion-request-log.md](./notion-request-log.md) 참고.

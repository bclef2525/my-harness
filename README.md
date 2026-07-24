# my-first-harness

에이전트와 스킬을 조합한 하네스를 모아나가는 프로젝트.
커밋 메시지 생성 하네스를 시작으로 계속 추가해나간다.

## 디렉터리 구조

- `.claude/agents/` — 에이전트 정의
- `.claude/skills/` — 스킬 정의 (에이전트를 조합하는 워크플로우)
- `_workspace/` — 중간 산출물

## 하네스 목록

### commit-message — 커밋 메시지 생성

2인 팀(author, reviewer)이 스테이지된 변경으로 커밋 메시지를 만든다.

- `commit-msg-author` — 커밋 메시지 초안 작성
- `commit-msg-reviewer` — 초안의 형식·사실을 검증하고 PASS/REDO 판정

"커밋 메시지 만들어줘"라고 요청하면 두 에이전트를 순차로 실행해
Conventional Commits 형식(`type(scope): subject`)의 메시지를 생성한다.

## 새 하네스 추가

1. `.claude/agents/`에 에이전트를 정의한다.
2. 필요하면 `.claude/skills/`에 에이전트를 조합하는 스킬을 정의한다.
3. 이 README의 **하네스 목록**에 항목을 추가한다.

# Rules
ADD-Drone팀 코드 관리 및 리뷰를 위한 규칙 모음

---

## Sections
- [Repository](#repository)
  - 관리
  - Naming rule
- [Commit](#commit)
  - log 작성 방법
  - commit 단위
- [Pull-Request](#pull-request)
  - 형상관리
  - issue 관리
  - pr 시점
  - merge 시점

---

## Repository
### 관리
특별한 경우가 아닌 이상 ***하나의 프로젝트, 또는 하나의 논문***에 대한 실험 진행시 ***하나의 레포지토리***만 사용

### Naming rule
레포지토리 생성시 아래 조건을 필수적으로 만족해야함
> 1) 영어
> 2) 소문자
> 3) 띄어쓰기 대신 - 사용
> 4) 구체적으로 작성

---

## Commit
### log 작성 방법
1. 아래의 7가지 유형중 1가지르 선택하여 로그 작성 시작
> 1. feat: 새로우 기능 추가
> 2. fix: 버그 수정
> 3. docs: 문서 파일 수정
> 4. style: 스타일 관련 기능(코드 포맷팅, 세미콜론 누락 등 코드 자체의 변경이 없는 경우)
> 5. refactor: 코드 리펙토링
> 6. test: 테스트 코드, 리펙토링 테스트 코드 추가
> 7. chore: 빌드 업무 수저, 패키지 매니저 수정(gitignore 수정 같은 경우)

2. 유형 선택 이후 동사형으로 시작하여 간결하고 직관적으로 작성
add, fix, modify, delete 등으로 시작

3. 예시
```
feat: add eegnet backbone network
docs: modify readme
chore: modify gitignore
```

### Commit 단위
커밋은 ***변경 사항에 대한 로그를 남기는것***이 주 목적이기 때문에 한번에 같은 기능을 실행할 때 필요한 파일들만 묶어서 ***최소한의 단위***로 진행

---

## Pull-Request
### 형상관리
코드 관리 및 리뷰를 위해 모든 프로젝트는 branch를 만들어서 작업진행

즉, ***main branch에 직접 commit 금지***

### issue 관리
새로운 기능, 실험 또는 기존 코드 수정 사항 등 모든 작업 진행시 해당 사항에 대해 반드시 ***issue 등록*** 후 commit 로그에 해당 issue 번호 추가
> 예시: `style: modify redundant code #61`

### PR 시점
***1-issue 1-pr 원칙***

pr 등록 이후, 코드 리뷰 요청

### Merge 시점
코드 리뷰 완료 댓글을 받은 이후에 코드 주인이 직접 merge

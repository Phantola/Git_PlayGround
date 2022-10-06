# Git_PlayGround

Phantola's git practice

### File Stage

git add [file]
git add \*

### File Stage cancel

git reset HEAD [file]

### File commit

git commit -m "[message]"

### Commit cancel

git reset [--soft, --mixed --hard] HEAD^(n)  
마지막 n 개 커밋을 취소

- soft : 취소된 해당 파일들을 stage 상태로 워킹 디렉토리에 보존
- mixed : 취소된 해당 파일들을 un-staged 상태로 워킹 디렉토리에 보존
- hard : 취소하고 해당 파일들을 un-staged 상태로 워킹디렉토리에서 삭제

### Commit Message change

git commit --amend

### Push

git push origin [branch-name]

### Push cancel

- 로그 확인
  - git log
- 원하는 시점으로 커밋 되돌리거나 시점으로 되돌림

  - git reset HEAD^(n)
  - git reset [commit id]

- 되돌려진 상테애서 커밋

  - git commit -m "message"

- 강제 푸시
  - git push origin [branch] -f

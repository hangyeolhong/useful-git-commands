## git status
1. untracked: 새로운 파일이고, git이 이 파일에 대해 아무것도 모름. 이 상태에서 `git add`를 하면 __staged__
2. staged: 이제 git이 파일에 대해 앎(**tracked 상태가 됨**), 다음 commit의 일부로 만듦
3. unchanged: 마지막 commit 이후 파일에 수정 사항이 없음. 이 상태에서 modify를 하면? __unstaged__
4. unstaged: 수정이 되었으나 다음 commit의 일부는 아님. `git add`를 하여 다시 stage할 수 있음

### 결론
* staged 상태로 만드려면 `git add` 명령을 실행해야 함
* `git add`는 파일을 새로 tracking할 때도 쓰이고 모든 파일을 stage 상태로 만들 때도 쓰임

### 참고
* commit하지 않은 파일을 untrack하고 싶으면? `git rm --cached <filename>`
* stage된 파일을 unstage하고 싶으면? (git add 취소) `git reset HEAD <filename>`
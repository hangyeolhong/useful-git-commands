## Rebase는 가장 까다로운 Git 명령어일까?

### git rebase
* 용도
    1. as an alternative to merging
    2. as a cleanup tool

### Merge vs Rebase
```
git switch feature
git rebase master # master 브랜치 위로 현재 브랜치를 올리는 작업
```

* rebase는 history를 다시 쓰는 것. 따라서 merge와 다르게, 깔끔하게 두 브랜치를 합병하는 것이 가능해짐
    * master 브랜치의 모든 커밋 이후에, current 브랜치의 모든 커밋을 이어짐

### Why Rebase?
* We get a much cleaner project history. No unnecessary merge commits! We end up with a linear project history.
---

### Interactive Rebase
* `git rebase -i HEAD~n`
    * pick: use the commit
    * reword: edit the commit message
    * fixup: meld it into previous commit and discard the commit message
    * drop: remove commit
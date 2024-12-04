## Commit

* Atomic Commits이란?
    * 각 커밋이 하나의 모든 작업을 포함하는 것 대신, 하나의 기능, 하나의 작업에 집중할 수 있도록 최대한 원자성을 유지하는 것이 중요

* Commit Messages는 **Present Tense**로 작성하기

* git log --abbrev-commit
* git log --oneline

* Amend
    * 바로 직전에 수행한 커밋만 amend 가능 
    * `git commit --amend`: 가장 최신 commit message를 편집할 수 있는 창이 뜸
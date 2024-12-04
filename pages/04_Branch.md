## Branch

* `git branch` view your existing branches
* `git branch <new-branch-name> <origin-branch-name>`
* `git switch -c <branch-name>`: 브랜치 만들고 해당 브랜치로 이동
* `git checkout -b <new-branch-name>`: 브랜치 만들고 해당 브랜치로 이동
---
### HEAD
* HEAD is simply a pointer that refers to the current "location" in your repository. It points to a particular branch reference.

---
### delete branch
1. 로컬 브랜치 삭제
```
git branch -d "로컬 브랜치명"
```

2. 원격 브랜치 삭제
```
git push "원격 저장소 이름" -d "원격 브랜치명"
예) git push origin -d "원격 브랜치명"
```

---
### git diff
`git diff branch1..branch2` will list the changes between the tips of branch1 and branch2

---
### 브랜치 삭제 및 이름 바꾸기
* `git branch -d <branch-name>`
* `git branch -D <branch-name>`: 강제 삭제
* `git branch -m <new-branch-name>`: 브랜치 이름 변경

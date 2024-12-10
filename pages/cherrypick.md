## 특정 commit만 merge 요청하고 싶을 때

### 설명
* 현재 **A branch**에서 작업 중이고 commit push를 여러 번 했음 -> 이 중에서 **develop 브랜치**에 특정 commit만 merge 요청하고 싶음

### 방법
1. git checkout develop
2. git cherry-pick <해당 커밋 해시값>
3. git push origin develop

* 만약에 충돌나면? git merge conflict 대응법 참고하기
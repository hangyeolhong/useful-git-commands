## Git stash
하던 작업을 임시로 저장해두고 싶을 때 사용하는 명령어

### 상황
* A branch에서 작업을 하다가, 다른 이슈가 생겨서 브랜치를 변경해야할 일이 발생
* 아직 A branch에서 작업이 완료가 안돼서 commit push하기가 좀 그럴 때, `git stash`를 사용


### git stash
* 우선 git add 해서 staged 상태로 만들어야함
* git stash하면 워킹 디렉토리에서 수정한 파일들만 저장함 --> 내 워킹디렉토리가 깔끔해짐
* 현재 브랜치에서 변경 사항을 스택에 저장했기 때문에, 이제 git checkout도 가능
* 기본적으로 **마지막 커밋 이름으로 stash 이름이 저장됨**
* 이름을 저장하고 싶으면 **git stash save "stash 이름"** 이렇게 하면 됨


### 명령어
* `git stash list`: 저장한 stash 목록 확인 가능
* `git stash apply / git satsh apply [stash 이름]`: 했던 작업 다시 가져오기
* `git stash drop`: 가장 최근의 stash 제거
* `git stash drop [stash 이름]`: stash 이름에 해당하는 stash 제거
* `git stash show -p | git apply -R`: 가장 최근의 stash를 제거하고, 다시 워킹디렉토리로 가져옴 (실수로 잘못 stash한 걸 되돌리고 싶을 때 사용)
* `git stash show -p [stash 이름] | git apply -R`: 특정 stash ...
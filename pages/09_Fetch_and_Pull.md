## Fetch and Pull


### Remote Tracking Branches
* 마지막으로 원격 저장소와 통신한 시간을 기억하는 포인터
* They follow this pattern `<remote>/<branch>`.
    * `origin/master` references the state of the master branch on the remote repo named origin.
    * `upstream/logoRedesign` references the state of the logoRedesign branch on the remote named upstream (a common remote name)
* `git branch -r`: view the remote branches our local repository knows about.
* `git checkout origin/master`: you can checkout these remote branch pointers
```
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
```

---
### git switch
* `git switch <remote-branch-name>` create a new local branch from the remote branch of the same name.
* e.g. `git switch puppies` makes me a local puppies branch AND sets it up to track the remote branch origin/puppies.
* `git switch` 이전에는 `git checkout --track origin/puppies`를 사용했음

---
### git fetch
* Workspace ---> `git add` ---> Staging (index) ---> `git commit` ---> Local Repository ---> `git push` ---> Remote Repository
* Local Repository <--- `git fetch` <--- Remote Repository
    * **현재 워킹 디렉토리에 반영되지 않음**
* Workspace <--- `git pull` <--- Remote Repository

* `git fetch <remote>` fetches branches and history from a specific remote repository. It only updates remote tracking branches.
    * e.g. `git fetch origin`
* `git fetch <remote> <branch>`: 단 하나의 브랜치만 fetching

---
### git pull
* Unlike fetch, pull actually updates our HEAD branch with whatever changes are retrieved from the remote.
    * "Go and download data from Github AND immediately update my local repo with those changes."
* git pull = git fetch + git merge
* `git pull <remote> <branch>`
* `git pull`: 자동으로 `git pull origin <로컬 브랜치명>` 이렇게 가져옴 (git switch로 remote branch를 tracking 한 상태라면)
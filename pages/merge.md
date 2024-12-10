## git merge

### 설명
* 내가 **A branch**를 만들고, A branch에서 작업하고 있었음
* 그런데 **develop 브랜치**의 내용이 업데이트되어서 **A branch**에 동기화를 해야하는 상황

### 방법
1. 현재 git branch는 **A**
2. **A branch**에서 현재 작업 중인 내용을 git add & git commit & **A branch**로 git push
2. git checkout develop ---> **develop 브랜치로 이동**
3. git pull origin develop ---> develop 브랜치 업데이트 내용 pull
4. git checkout A ---> **다시 A 브랜치로 이동**
5. git merge develop ---> develop 브랜치 내용을 A 브랜치에 합치기
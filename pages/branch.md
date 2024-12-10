1. 모든 원격 브랜치 가져오기(fetch)
`git fetch origin`

2. 체크아웃할 수 있는 브랜치 목록 보기
`git branch -a`

3. 원격 브랜치 가져와 병합하기(Pull)
원격에서 만든 브랜치를 로컬로 가져와서 작업을 수행해야 하므로 원격 브랜치를 가져오기

`git checkout -b feature/test origin/feautre/test`

로컬에 feature/test라는 새 브랜치를 생성하고,
새 브랜치로 체크아웃이 되며,
origin/feature/test를 새 브랜치로 가져옴
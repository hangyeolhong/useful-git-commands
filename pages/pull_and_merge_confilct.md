운영 서버 main 브랜치에서, `git pull origin main` 했을 때, 

json이나 pkl에서 merge conflict가 생긴다 --> 원격 저장소의 파일들로 덮어쓰고 싶음

1. 로컬 변경 사항 스태시
* `git stash push -m "메시지" /src/assets/*`

2. 다시 pull (로컬의 json, pkl 변경 사항이 스태시되었기 때문에, pull해도 충돌이 안남)
* `git pull`

3. 가장 최근의 스태시 제거
* `git stash drop`
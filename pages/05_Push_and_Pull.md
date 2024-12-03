## git push, pull

`git push -u origin [브랜치명]`
* 현재 checkout한 브랜치와, 원격의 [브랜치명] 브랜치를 tracking connection
* 이후에 `git push`, `git pull`만 해도, 자동으로 원격의 [브랜치명] 브랜치에 push, pull함

`git push origin [브랜치명]`
* 현재 checkout한 브랜치를 원격의 [브랜치명] 브랜치에 push

`git pull origin [브랜치명]`
* 현재 checkout한 브랜치로 원격의 [브랜치명]을 가져옴

`git push origin develop:main`
* 로컬 브랜치 develop을 원격의 main 브랜치에 push

`git pull origin main:develop`
* 원격 저장소의 main 브랜치를 로컬 브랜치 develop에 pull
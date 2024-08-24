## git log

1. 깃 로그를 보자

```
git log --since="2 days ago"
git log --since=2.weeks
git log --since="2 years 1 day 3 minutes ago" # 자유롭게 가능
```

* --oneline: 각 커밋을 한 줄로 압축하여 표시
* --author=[이름]: 특정 저자의 커밋만 표시
* --since=[날짜]: 특정 날짜 이후의 커밋만 표시
  
2. git reset으로 해당 작업 환경으로 돌아가기
* `git reset --soft [커밋 번호]`: 변경 내용 유지하면서, 커밋을 이전 상태로 되돌림
* `git reset --hard [커밋 번호]`: 변경 내용을 완전히 삭제하고, 커밋으로 덮어쓰기
* 디폴트는 `git reset --mixed`
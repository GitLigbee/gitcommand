> git fetch 将远程分支更新取回到本地,还没有合并到工作区

- 将与本地分支关联的远程分支的更新全部取回到本地
`git fetch origin`

- 获取指定分支更新
```
git fetch origin branchName

; 取回更新后，会返回一个FETCH_HEAD ，指的是某个branch在服务器上的最新状态，我们可以在本地通过它查看刚取回的更新信息
git log -p FETCH_HEAD
; 将拉取下来的最新内容合并到当前所在的分支中
git merge FETCH_HEAD
```

> git pull 将远程分支更新取回到本地,并合并到工作区，相当于 git fetch + git merge

- 拉取更新合并指定分支
```
git fetch origin remoteBranchName:localBranchName
git fetch origin remoteBranchName ; 与当前分支合并，可省略:
```
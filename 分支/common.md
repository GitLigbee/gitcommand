> 创建分支
`git branch branchName`

> 切换分支
`git checkout branchName`

> 创建并切换分支
`git checkout -b branchName`

> 删除分支
```
git branch -d branchName ;删除本地分支

git branch -d -r branchName ;删除远程分支，删除后还需要推送到远程服务器
git push origin:branchName
```

> 重命名
`git branch -m oldName newName ;本地分支`

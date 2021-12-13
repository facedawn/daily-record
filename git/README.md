使用access token进行push，用户名为github用户名，密码为developer setting里面生成的token

git push origin master

git checkout master //切换主分支

git merge dev //将dev分支合并到当前分支

git checkout -b dev //dev为分支名称，先创建再切换

git checkout -b dev origin/master //从远程master支拉取一个dev分支

git branch -a //会把远程的分支也显示出来

git breanch //显示本地分支

git rebase master //在哪个分支上把master更新到当前分支上

git remote -v //查看远程仓库地址

git remote add upstream git@github.com/xxxx.git //添加远程仓库

git fetch upstream

git merge upstream/main


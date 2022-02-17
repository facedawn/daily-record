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

# git clone 指定分支
第一步： git clone [git-url] -b [branch-name]

第二步：git reset --hard [commit-number]    //回退几个commit版本


# git clone 时GnuTLS recv error(-110)
git clone  --recursive https://xxxxx

# git clone 指定版本号的版本
切换到指定的版本号：

git checkout 17def2f

新建分支

git checkout -b branch

这时候，就下载到你想要的版本的代码了。

# git clone 时 server certificate verification failed. CAfile: /etc/ssl/certs/ca-certificates.crt CRLfile: none
关闭系统的安全认证。
能解决所有证书问题，操作简单，系统面临一定的风险。
export GIT_SSL_NO_VERIFY=1

# 该命令直接放弃所有修改代码,并更新到版本库最新版本代码;
1. git fetch --all
2. git reset --hard origin/master
3. git pull

# OpenSSL SSL_read: Connection was reset, errno 10054
换到终端push

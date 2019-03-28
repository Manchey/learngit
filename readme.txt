touch <Name>.txt	create a txt file

初始化
git init

添加
git add <fileName>
git commit -m “comments”

git status
git diff <fileName>		check the differences
git reset HEAD <fileName>	cancel the temporal storage of <fileName>

git log
git log --pretty=oneline
git reflog

HEAD				current version
HEAD^				
HEAD^^
HEAD~100

修改
git reset __hard HEAD^
git checkout -- <fileName>	撤销<fileName>的最近更改，回到上一次commit or add的状态
git reset HEAD <fileName>	撤销暂存区的修改


删除
rm <fileName>
git rm <fileName>
git commit -m “comments”	删除
git checkout -- <fileName>	恢复


远程仓库
.ssh
id_rsa			私钥
id_rsa.pub		公钥

git remote add origin git@server-name:<userName>/<repName>.git
git push -u origin master
git clone git@github.com:<>/<>.git
git remote remove origin
git remote -v


分支管理
git checkout -b dev	创建并切换到dev分支

git branch dev		创建dev分支
git checkout dev	切换到dev分支

git branch		查看分支状态

git check out master	回到主分支
git merge dev		合并dev到主分支
git branch -d dev	删除dev分支

git log —graph		查看分支合并图
git merge --no-ff -m “…”	不用快速合并


修复bug
git stash			临时储存当前工作
git stash list			查看储存
git stash apply			恢复
git stash drop			删除
git stash pop			恢复并删除
git stash apply stash@{0}	



解决冲突
git pull
git branch --set-upstream-to = origin/dev dev

标签管理
git tag <name>
git tag
git tag <name> <commitId>
git show <tagname>
git tag -a <name> -m <message>
git tag -d <name>

配置别名
git confit —global alias.st status
touch <Name>.txt	create a txt file

��ʼ��
git init

���
git add <fileName>
git commit -m ��comments��

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

�޸�
git reset __hard HEAD^
git checkout -- <fileName>	����<fileName>��������ģ��ص���һ��commit or add��״̬
git reset HEAD <fileName>	�����ݴ������޸�


ɾ��
rm <fileName>
git rm <fileName>
git commit -m ��comments��	ɾ��
git checkout -- <fileName>	�ָ�


Զ�ֿ̲�
.ssh
id_rsa			˽Կ
id_rsa.pub		��Կ

git remote add origin git@server-name:<userName>/<repName>.git
git push -u origin master
git clone git@github.com:<>/<>.git
git remote remove origin
git remote -v


��֧����
git checkout -b dev	�������л���dev��֧

git branch dev		����dev��֧
git checkout dev	�л���dev��֧

git branch		�鿴��֧״̬

git check out master	�ص�����֧
git merge dev		�ϲ�dev������֧
git branch -d dev	ɾ��dev��֧

git log ��graph		�鿴��֧�ϲ�ͼ
git merge --no-ff -m ������	���ÿ��ٺϲ�


�޸�bug
git stash			��ʱ���浱ǰ����
git stash list			�鿴����
git stash apply			�ָ�
git stash drop			ɾ��
git stash pop			�ָ���ɾ��
git stash apply stash@{0}	



�����ͻ
git pull
git branch --set-upstream-to = origin/dev dev

��ǩ����
git tag <name>
git tag
git tag <name> <commitId>
git show <tagname>
git tag -a <name> -m <message>
git tag -d <name>

���ñ���
git confit ��global alias.st status
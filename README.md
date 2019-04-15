1 git的指令：
2 git init #创建git管理的版本库！（要在当前目录下进行）
3 git add name  #增加文件到版本库
4 git commit -m "xx"  #提交文件到版本库（命令可以一次上传多条文件，xx为备注）
5 git status  #查看库内文件状态（红色为未进行add增加进入版本库，绿色为已经增加但未提交）
6 git log   #查看记录
7 git reset --hard HEAD^  #回退到上一个版本（git中HEAD表示当前版本HEAD^表示上一个版本，HEAD^^表示上上个，同样可以用HEAD~n表示回退n个版本）
8 git reflog #查看版本号方便进行回退
9 git checkout -- file  #撤销工作区的修改（让文件回到最近一次git add或git commit状态）
10 git rm file  #删除文件
11 git push -u origin master  #将本地的master分支推送到远程仓库的master分支上
12 git remote add  origin git@server-name:path/repo-name.git #将本地和远程仓库关联起来
13 git clone git@github.com:name/file.git  #将远程的仓库克隆下载到本地其中name为注册的github账号名；file为想要克隆的仓库名
14 git branch name 创建一个新的分支name为分支名(分支存在于本地版本，需要使用git push才能其推送至远程)
15 git checkout name  切换到该分支下
16 git checkout -b name  #创建一个新的分支并切换到该分支 相当于14+15；
17git branch  查看分支；当前分支会有*标记
18 git checkout name 切换分支
19 git merge name  合并分支（将name分支的内容合并到当前分支上）
20 git branch -d name 删除name分支将d换成D为强制删除
21
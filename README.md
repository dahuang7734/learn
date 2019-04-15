git的指令：
git init #创建git管理的版本库！（要在当前目录下进行）
git add name  #增加文件到版本库
git commit -m "xx"  #提交文件到版本库（命令可以一次上传多条文件，xx为备注）
git status  #查看库内文件状态（红色为未进行add增加进入版本库，绿色为已经增加但未提交）
git log   #查看记录
git reset --hard HEAD^  #回退到上一个版本（git中HEAD表示当前版本HEAD^表示上一个版本，HEAD^^表示上上个，同样可以用HEAD~n表示回退n个版本）
git reflog #查看版本号方便进行回退
git checkout -- file  #撤销工作区的修改（让文件回到最近一次git add或git commit状态）
git rm file  #删除文件
git push -u origin master  #将本地的master分支推送到远程仓库的master分支上
git remote add  origin git@server-name:path/repo-name.git #将本地和远程仓库关联起来

###创建一个版本库
midir learngit  #在当前目录下新建一个文件夹作为一个版本库
cd learngit 	# 进入当版本库文件夹下
pwd 			#读取当前路径

git init 		#将当前目录初始化为可以管理的仓库


git add file.txt
git commit -m "add text"
git status 		##获取当前版本库是否都上传


git diff 		#查看当前版本与上一个版本之间有什么差别
git log  		# 查看之前的版本号
git log --pretty=oneline 		#只查看查看之前版本号
`
git reset Head^					#版本回退，一个^代表一个版本，、
git reset Head^^ 				# 往上前两个版本
git reset Head~100				# 往上一百个版本

cat file.txt					# 查看该文件的内容

git reflog 						#查看历史命令，方便自己查看返回到那个版本的

ESC +ZZ 						# 退出git中的vim编辑器

git restore --staged file.txt	#将加入到暂存区的文件撤回
git checkout -- file.txt		#丢弃掉工作区的修改，如果没有加入暂存区，则回到和版本库一样的状态，如果加入到暂存区，则回到和add中的文件一样的状态。

git rm file.txt						#删除文件管理库中的文件,在没有使用git commit 之前可以通过 git checkout -- file从暂存区撤回，


git remote add origin git@github.com:INeverSayNever/learngit.git  # 远程连接GitHub库

git push -u origin master 			#第一次推送本地文件时
git push origin master				#将本地库上传到github


Git has a mutable index called stage.
Git tracks change.


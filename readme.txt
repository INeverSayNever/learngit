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


Git has a mutable index called stage.
Git tracks change of files.


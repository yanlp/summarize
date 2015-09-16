# summarize
 summimg up some questions
总结项目中遇到的问题

1、生成ssh秘钥指导网址:
	https://help.github.com/articles/generating-ssh-keys/
命令:
    ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
2、git的命令集合
	mkdir **  创建新目录
	git init  初始化本地仓库
	git remote add github git@github.com:yanlp/lipsky.git
		git remote -v
			github  git@github.com:yanlp/lipsky.git (fetch)
			github  git@github.com:yanlp/lipsky.git (push)
	git remote add origin git@github.com:yanlp/lipsky.git
		git remote -v
			origin  git@github.com:yanlp/lipsky.git (fetch)
			origin  git@github.com:yanlp/lipsky.git (push)
	添加远程仓库路径

ps: fatal:remote origin already exists.
: git remote rm origin
ps: 删除文件夹
  git rm --cached */src/\*文件名
  git commit -m 'remove 文件'
  git push origin master 提交到远程服务器
ps:.gitignore 文件可以设置不希望提交到远程的文件
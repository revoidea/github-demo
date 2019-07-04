##### git bush的命令行
- cd 改变目录
- mkdir 创建目录
- pwd 打印目录
- mv 移动文件
- cp 复制文件
- rm 删除文件
- ls .. 返回上一层目录

##### linux 命令
- 写入内容并创建内容
echo 'xxxx' > xxxx（文件）
- 打印文件内容
cat

##### 设置git全局参数
- 显示当前的git配置
git config --list
- 设置提交仓库时的用户名信息
git config --global user.name  "xxxx"（可为中文名）
- 设置提交仓库时的邮箱信息
git config --global user.email "xxxx" (建议用github上注册的账号)

##### git命令
- 1.新建代码仓库
- 在当前目录新建一个git代码库
git init
- 下载一个项目和它的整个代码历史
https://github.com/[userName]/reposName
git clone [url]

- 2.添加/删除/修改文件
- 添加指定文件到暂存区
git add [file1] [file2](或者 git add .)
- 删除工作区文件，并且将这次删除放入暂存区
git rm [file1] [file2]

- 3.改名文件，并且将这个改名放入暂存区
git mv [file-origin] [file-renamed]

- 4.代码提交
- 提交暂存区到仓库
git commit -m [message]
- 直接从工作区提交到仓库(前提该文件已经有仓库中的历史版本)
git commit -a -m [message]

- 4.查看信息
- 显示变更信息
git status
- 显示当前分支的历史版本
git log
git log --oneline

##### 同步远程仓库
- 增加远程仓库，并命名
git remote add [shortname] [url]

- 将本地的提交推送到远程仓库
git push [remote] [branch]

- 将远程仓库的提交拉下到本地
git pull [remote] [branch]

- 从本地提交到远程仓库
git push origin master


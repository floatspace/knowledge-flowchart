# 基本命令
git init  初始化一个版本仓库  
git clone yourgitaddress 克隆远程版本仓库到本地  

git remote add origin yourgitaddr 本地添加远程版本库origin  
git remote -v  查看远程仓库  

git add .   将文件的修改，文件的新建，添加到暂存区
git add -u  将文件的修改、文件的删除，添加到暂存区
git add A   将文件的修改，文件的删除，文件的新建，添加到暂存区

git commit -m "注释内容"  提交修改  

git push origin master  将当前分支推送到origin主机的对应分支  git push [远程名] [本地分支]:[远程分支]  
git push -u origin master 如果当前分支与多个主机存在追踪关系，则可以使用 -u 参数指定一个默认主机，这样后面就可以不加任何参数使用git push  

git status 查看文件状态  
git add newfile.txt 跟踪新文件  
git rm newfile.txt  从当前跟踪列表移除文件，并完全删除  
git rm --cached newfile.txt 仅在暂存区删除，保留文件在当前目录，不再跟踪

git mv newfile.txt a.txt  重命名文件  
git mv newfile.txt newfolder 移动文件至文件夹
 
git log 查看提交的历史记录  

# 分支管理
git branch workspace  创建一个分支  
git checkout workspace 切换工作目录到workspace  
git checkout -b workspace  上面两个命令的合并，创建workspace分支并切换到workspace  

git merge workspace 合并workspace分支，当前工作目录为master  
git branch -d workspace 合并完成后，没有出现冲突，删除workspace分支  

git fetch 拉取远程仓库的数据，语法：git fetch [remote-name]  
git pull fetch会拉取最新的远成仓库的数据，但不会自动到当前目录下，需要pull自动合并  

git remote show origin 查看远程仓库的信息  

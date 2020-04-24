#### 1、git常使用命令

git config --global user.name "zhanghongxu"
git config --global user.email "1085360155@qq.com"
git status
git log 
git log --decorate
git add *    添加所有 
git commit -m " "
git reset HEAD`     将上一个版本回到暂存区域
git reset --hard HEARD 将上一个版本还原到工作目录
git diff id1  id2     比较两个快照的区别
git branch feature    创建分支feature 
git checkout feature    切换分支feature 
git checkout -b feature2    新创建并切换分支feature2 
git merge feature2   合并分支
git log --decorate --all --oneline --graph
git branch -d feature  删除分支

git push 本地同步到远程
git pull origin master -f    强制

git reset --hard origin/master     把HEAD指向master最新版本，强制拉去

git clone git@github.com:zhhx1101/git-note.git

#### 2、git本地同步到远程

1、在要同步的文件中使用：git init 

2、将程序保存在本地git的暂存区，使用 git add *  

3、将程序保存在本地的git库，使用git commit -m "     "

4、git remote add origin git@github.com:zhhx1101/xinqiu.git

5、git push origin master，本步骤如果报错Updates were rejected ......,就使用git push origin master -f

#### 3、只拉取github中的某个文件夹

1、线在本地创建文件夹，然后git init，git remote add -f origin git@github.com:zhhx1101/xinqiu.git;

2、git config core.sparsecheckout true

3、echo 文件夹名 >> .git/info/sparse-checkout

4、git pull origin master 



分支推送顺序的写法是<来源地>:<目的地>

https://www.cnblogs.com/dyh-air/p/9257237.html


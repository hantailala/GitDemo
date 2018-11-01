# GitDemo
Git 是一个版本控制工具

GitHub 是一个托管 Git 项目的服务

1.git remote 的输出只是一个单词origin（简写名），"origin" 一词是指代主远程仓库的专用名称。

2.git remote -v 查看当使用origin一词时，实际上使用的是路径。

3.git remote add 用于创建一个origin简写名，指向github上的项目，运行git remote -v 会显示简写名和URL。

4.git log --oneline --graph --decorate --all 显示commit日志，跟踪分支。

5.git add . 添加文件

6.git commit -m 'xxx'  提交本地

7.git push <remote-shortname> <branch> 将本地的提交推送到远程仓库，你需要提供远程仓库简写名及用于容纳你的提交的分支名。如：git push origin master
  
8.git pull <remote-shortname> <branch> 将远程的代码同步到本地。
  1.获取远程更改（这会将 commit 添加到远程仓库，并移动跟踪分支指向它们）
  2.本地分支与跟踪分支合并
  
9.git fetch 用于从远程仓库分支检索 commit ，但不会在收到这些 commit 之后，自动将本地分支与远程跟踪分支合并。
  git fetch origin master
  运行 git fetch 后，会发生以下活动：
  远程分支上的 commit 会复制到本地仓库。
  本地跟踪分支（例如，origin/master）移到指向最新的 commit。
  你可以将 git fetch 想象成 git pull 它的一半操作，而 git pull 的另一半是合并。
10.git merge origin master 合并

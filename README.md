# GitDemo
Git 是一个版本控制工具

GitHub 是一个托管 Git 项目的服务

1.git remote 的输出只是一个单词origin（简写名），"origin" 一词是指代主远程仓库的专用名称。

2.git remote -v 查看当使用origin一词时，实际上使用的是路径。

3.git remote add 用于创建一个origin简写名，指向github上的项目，运行git remote -v 会显示简写名和URL。

4.git log --oneline --graph --decorate --all 显示commit日志，跟踪分支,分页，按Q退出。

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
  
10.git merge origin master 合并。

11.git show SHA 显示那次提交信息。

12.git tag -a v1.0 -m 'xxxx' 带注释的标签，因为它们包含了大量的额外信息，包含创建者，日期，信息。 git tag -a v1.0 a87984向以前的提交打tag

13.git tag -d v1.0.0 删除标签。

14.git tag 验证标签是否已经添加了tag。

15.git branch 列出仓库中的所有分支名称、创建新的分支、删除分支。

16.git branch -d sidebar 删除分支

17.git branch 名称  创建分支。

18.git checkout 分支名  切换分支。

19.git merge <other-branch> 合并分支。

20.git commit --amend 修改最后一个commit。

21.git revert <SHA-of-commit-to-revert> 命令用于还原之前创建的 commit

22.git reset <reference-to-commit> 将 HEAD 和当前分支指针移到目标 commit，清除 commit，将 commit 的更改移到暂存区，取消暂存 commit 的更改

参考视频：https://classroom.udacity.com/courses/ud123

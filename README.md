# GitDemo
Git 是一个版本控制工具

GitHub 是一个托管 Git 项目的服务

1.git remote 的输出只是一个单词origin（简写名），"origin" 一词是指代主远程仓库的专用名称。

2.git remote -v 查看当使用origin一词时，实际上使用的是路径。

3.git remote add 用于创建一个origin简写名，指向github上的项目，运行git remote -v 会显示简写名和URL。

4.git log --oneline --graph --decorate --all 显示commit日志。

5.git add . 添加文件

6.git commit -m 'xxx'  提交本地

7.git push <remote-shortname> <branch> 将本地的提交推送到远程仓库，你需要提供远程仓库简写名及用于容纳你的提交的分支名。如：git push origin master
  
8.  

# git

New repository的时候我想已经提示的很清楚你下一步该怎么做了。。。

#####我觉得只要分清楚：工作区——版本库——远程库。一般不会有问题的，除非是冲突

    1、git checkout dev 
    
    创建一个分支，在分支上开发，叫工作区
    
    1.1、git status
    
    查看工作区改动.h或者.m
    
    2、git add
    
    git add + 类名或者 + 文件名  (暂存区)
    
    git add . (添加全部代码修改到暂存区)
    
    git add -A (添加全部文件夹修改到暂存区)
  
    git commit -m 叫版本库
    
    3、git push origin master
    
    推到远程仓库
    
    1.首先多人开发要在自己创建的分支上开发
    
    2.push之前切换到master分支先将最新的pull下来，在合并自己的分支 
    
    3.如果存在冲突，解决冲突后再push
    
    4.在push之前最好看看修改了什么，一些没修改的只查看了也会改版本号的就不用add了，可以避免冲突

#####一般会用到的git操作
       
    1、git diff 
    
    查看修改的类
    
    2、git log
    
    从最近到最远的提交日志
    
    3、git reset -- hard HEAD^
    
    返回上一版本
    
    4、git reflog
    
    你的每一次命令
    
    5、git checkout -- .
    
    回到版本库最新版本，除非你不想要的更改，否则别轻易尝试，一般忽略就git checkout + 类名
    
    6、git branch
    
    查看当前分支
    
    7、git merge + 分支
    
    合并分支
    
    8、git checkout -b +分支
    
    创建分支并切换分支等同于 git branch +分支和git checkout +分支
    

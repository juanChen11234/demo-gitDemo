# demo-gitDemo
study git

##  $ git reflog
 >查看提交历史

##  $ git reset --hard 3628164
 >版本更改

## 撤销没有被git add的修改,包括删除
 > $ git checkout -- 1.html <br/>
 >git checkout其实是用版本库里的版本替换工作区的版本 <br/>
 >（git checkout -- file命令中的--很重要，没有--，就变成了“切换到另一个分支”的命令）

## *【撤销已经git add到暂存区的修改
 >先：$ git reset HEAD 1.html <br/>
 >再：$ git checkout -- 1.html

## 查看当前的分支
 >$ git branch

## 创建分支并切换到分支上
 >$ git checkout -b dev <br/>
 >(相当于：$ git branch dev(创建分支) + $ git checkout dev(切换到分支))


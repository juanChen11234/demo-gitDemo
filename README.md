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

## 撤销已经git add到暂存区的修改
 >先：$ git reset HEAD 1.html <br/>
 >再：$ git checkout -- 1.html

## 查看当前的分支
 >$ git branch

## 创建分支并切换到分支上
 >$ git checkout -b dev <br/>
 >(相当于：$ git branch dev(创建分支) + $ git checkout dev(切换到分支))

## 合并A分支到B分支
 >先：切换B到分支 <br/>
 >再：$ git merge A分支的名字

## 删除分支
 >$ git branch -d 分子名字

## 解决冲突
 >如果对两个有冲突的分支执行--分支的合并--操作 <br/>
 >会看到：CONFLICT (content): Merge conflict in readme.txt 。(readme.txt 文件冲突了)<br/>
 >怎么办呢？<br/>
 > <font color="#A52A2A">Git用<<<<<<<，=======，>>>>>>>标记出不同分支的内容</font><br/>
 > 1、在冲突文件中修改git 标记出来的冲突部分。<br/>
 > 2、执行$ git add readme.txt , $ git commit -m 'xxx'


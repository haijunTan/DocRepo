1.初始化一个Git仓库，使用git init命令。  

2.添加文件到Git仓库，分两步：  
  第一步，使用命令git add <file>，注意，可反复多次使用，添加多个文件；  
  第二步，使用命令git commit，完成。    

3.随时掌握工作区的状态，使用git status命令。    

4.如果git status告诉你有文件被修改过，用git diff可以查看修改内容。  

5：版本回退：  
  a.HEAD指向的版本就是当前版本，因此，Git允许我们在版本的历史之间穿梭，使用命令git reset --hard commit_id。  
  b.用git log可以查看提交历史，以便确定要回退到哪个版本。  
  c.要重返未来，用git reflog查看命令历史，以便确定要回到未来的哪个版本。  

6.撤销修改：  
  场景1：当你改乱了工作区某个文件的内容，想直接丢弃工作区的修改时，用命令git checkout -- file。   
  场景2：当你不但改乱了工作区某个文件的内容，还添加到了暂存区时，想丢弃修改，分两步：  
        第一步用命令git reset HEAD file，就回到了场景1，  
        第二步按场景1操作。  
  场景3：已经提交了不合适的修改到版本库时，想要撤销本次提交，参考版本回退一节，不过前提是没有推送到远程库。  

7.Git鼓励大量使用分支：  
  查看分支：git branch
  创建分支：git branch <name>  
  切换分支：git checkout <name>
  创建+切换分支：git checkout -b <name>
  合并某分支到当前分支：git merge <name>
  删除分支：git branch -d <name>

8.打标签：   
  git tag <name>用于新建一个标签，默认为HEAD，也可以指定一个commit id；   
  git tag -a <tagname> -m "blablabla..."可以指定标签信息；   
  git tag -s <tagname> -m "blablabla..."可以用PGP签名标签；  
  git tag可以查看所有标签。  
  git push origin <tagname>可以推送一个本地标签；  
  git push origin --tags可以推送全部未推送过的本地标签；  
  git tag -d <tagname>可以删除一个本地标签；  
  git push origin :refs/tags/<tagname>可以删除一个远程标签。  

  ref:http://www.liaoxuefeng.com/wiki/0013739516305929606dd18361248578c67b8067c8c017b000

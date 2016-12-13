###Git Command
(Infrun : Git & Redmine)

##1. Git 작업공간
	Working? - Stage - Commit

##2. Command
>>git status			==> 현재 작업공간 상태
>>git add xxx			==> xxx 파일을 stage 공간으로 이동
>>git commit -m 'add xxx file' ==> xxx 파일을 commit 공간으로 이동
>>git branch			==> shows branch status
	master
	t1
	t2
	*t3		(현재 checkout되어 있는 branch)
>>git checkout -b t1	==> t1 branch checkout
>>git branch -m t1 a1	==> t1 branch를 a1으로 변경
>>git branch -d a1 		==> a1 branch삭제
>>git merge t2			==> t2 branch를 현재 branch와 merge

##3. remote repository commit
>>git clone https://id:pw@github.com/yuriyaya/Study.git

##4. Github 설명

**<아무 파일도 없을 때>**
echo "# Study" >> README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin https://github.com/yuriyaya/Study.git
git push -u origin master

**<파일이 있을 때>**
git remote add origin https://github.com/yuriyaya/Study.git
git push -u origin master

local에서 파일을 commit 한 후 remote로 push하면 됨...
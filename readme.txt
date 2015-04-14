this is just a test repo!

======================== commit a new project to repo ========================
$ cd myproject

$ git init

$ git add .
	add current directory and any file into repo
	
$ git commit -m 'initial commit'
	commit staged files to local repo

======================== manage remote connection info ========================
$ git remote -v
	display remote URLs
	
$ git remote add origin git@gitserver:/opt/git/project.git
	make(log) connection to some remote server

======================== make change and commit to repo ========================
$ git add filename1
$ git add filename2
$ git commit -m 'modified something'





======================== check status ========================
$ git status
======================== view unstaged change ========================
$ git diff
======================== view uncommited staged change ========================
$ git diff --stage
 !!!recommend use Git GUI tools from gitk instead !!!

 
 
 
======================== view history info ==========================
$ git log
 !!!recommend use Git history tools from gitk instead !!!

 
 
 
======================== upload to server ========================
$ git push origin master
	final push


	
?<<<<<<< HEAD
	============= some change on mater brunch ===============
?=======

	========================= dev2 brunch for another programmer ============
	git checkout -b dev2

	dev2.step2
?>>>>>>> dev2




	

?<<<<<<< HEAD
	
	dev3 do modification on master when the actuall remote/origin/master is advanced already by dev2.
	when he try to push local master into remote, there is an error.
	because remote/origin/master is modified simutaniously as dev3 do the work.
	dev3 can only fetch remote master first and try to merge use "git merge origin"
	

?=======

	dev2 do some mofidy on master
	so master branch will be advanced than remote/origin/master normally.
	actually remote/origin/master will not move if we donnot pull/push with remote.

	dev2's modification is pushed first, and sucessed

	dev3 will need "git merge origin" before he can push to origin!!!
?>>>>>>> origin/master

	

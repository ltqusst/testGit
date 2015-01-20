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
	

	
	
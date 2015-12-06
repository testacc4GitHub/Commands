#git commands
####setting up a local and remote repo for the <b>1st time</b>
``` sh
$ git init
$ git add filename
$ git commit -m "comment"
$ git remote add origin master http://github.com/username/reponame.git
$ git push -u origin master
```
####pushing changes made from file(s) to the remote repo
``` sh
$ git add . // or $ git add filename
$ git commit -m "comment"
$ git push // *user origin* not needed because of *-u...* in setting up
``` 
####erasing a single file from git
Erase the file from the local repo as normal, then, when using the command **_git add ._**, change it to this:
``` sh
$ git add . --all
```

Another way to do it:  delete the file, then use this command:
``` sh
$ git add -u
```
Then when you commit, it will commit the deleted file.




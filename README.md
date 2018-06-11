
	 #GIT TUTORIALS

	___________________________________________________

	*****When you start your new project *********

	git init 
	git remote add origin 'url'
	git status  - git status kuch code he, uncommited 
	git stash 
	git pull 
	git stash apply
	git add . 
	git commit -m "Message"
	git push origin development 
	git stash clear 
 
    ______________________________________________________________
     After that you need to follows these steps daily.
 	git status
	git add .
	git commit -m "mesage"
	git push origin development

	_________________________________________________________________________
     How  To Solve Merge Conflicts *** Created by Anup Choudhary Date:11-06-18 **
     
     Let suppose assume you are making changes in your project or branch and you forget to check git status and you made commit in your project and you try to push your code into bitbucket and it gave you error because your online project is ahead of one head and now you want to solve the conflict in it.Let follow the following steps which help you to solve merge conflicts.
    
     1.git log --online
        48db27b (HEAD -> master) added index3
		abf10b8 added index
		ee7fcb7 index.html edited online with Bitbucket
		b8f4ab8 Added initial commit
		cc5e39f Initial commit

     2.Match your latest commit with online commit and i found that latest commit which match my online commit was abf10b8.
    
     3.Now we have to reset the 48db27 commit id.
              git reset HEAD~1
    
     4.when your will check now with git log --online you will see that now your current head is abf10b8.
    
     5.Now you check git status and you will see there is untracked files in your system and now you want to save the changes.
     
     6.Before saving changes check whether your stash is empty or not with following command
                    git stash list
    
     7.If it is not empty then clear your stash with following command
               git stash clear
     
     8.when your clear your stash added latest changes into your stash with following command
                git stash
     
     9.Now you check your git status and you will find that nothing to commit.
    
     10.so now you can pull your online code into your git repository with following command
                git pull origin master
     
     11.Then after again check your git status and you will find nothing to commit.
    
     12.So now you can apply your modified changes which are in stash with following command
                   git stash apply.
     
     13.Then after use git add . and git commit -m "with message"
     
     14.Then again check git status and if you find nothing to commit then push your code to online repository with following command
                 git push origin master



	
___________________________________________________________________________________________
	

	git log --oneline -5				to check what history of the project last five(5)

	git reset --hard 2bf922b(git commit id)					------to delete forcely

	git reset --soft 2bf922b(git commit id)					------to take locally

	git branch

	git branch dev

	git branch

	git checkout dev

	git cherry-pick ed3a0d8(git commit id)			to copy commit from one branch to another

	git log --oneline -5							to get last five commits

	git pull origin master							to first get commits to local syatem


	git reset --soft 2bf922b						to make local commit reset softly when push gives rejected error

	git stash list

	git stash 9f23b31

	git stash apply

	git stash clear

	git stash list
	git stash clear
	git status
	git reset --soft id

	git status
	git stash list

	git stash
	git stash list
	git pull origin master

	git stash apply
	git stash clear
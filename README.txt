This is Lisa's great FVCOM code

  how to compile:

	1)edit makefile
	2)make clean
	3)make

 How to clean up

	make clean
	rm *.f90
	
 How to add new stuff to github:

	vi newfile.F # //for example

	git add newfile.F

	git commit -m "Lisa created a new file named newfile.F" 

	git push origin master

   
How to update an old file 

	vi oldfile.F
	git add -u .

	git commit -m "Lisa updated oldfile.F for xyz reasons"

	git push origin master 

How to pull from githbub

	git pull origin master

How to create a new branch and do some cool stuff


        git checkout master #switch to master branch on local machine
	git pull #to make sure master on local machine the latest from the github

	git branch my-new-branch  #creating a new branch based on master


	vi files.F 	#change any file you want 

	git add -u .   # commit that files.F file if files.F was old

	#or 
	git add files.F #if files.F is new
	git commit -m "Lisa created new branch edited files.F"

	git push origin my-new-branch   #this pushes this new branch to github with also a branch name my-new-branch

	
	#then merge master into this new branch if you need, in case someone else change master already during your work on this branch

	git checkout master #switch back to master
	git pull            #update your master on local machine to be same as on github

	git checkout my-new-branch  # get back to the new branch again

	git merge master    #merges new stuff in the master just pulled, into the new branch here

	git commit -m "lisa merged what is new the master branch to this new branch named my-new-branch" 

	git push origin my-new-branch #push this new branch that has the latest master as well to the github again in the remote branch also named my-new-branch


	#then  ask the github to merge the new branch into master on github by
        #a) visit github.com 
	#b) find the my-new-branch
        #c)  create a "pull request"
        #d) review the pull request, make sure nothing wrong
        #e) approve the pull request

	#finally pull the latest master on the github back to the local master again
	
	git checkout master #switch back to master agian on local machine
	git pull origin master  #pull the latest master from github 

	

	


	



	

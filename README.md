# EmployeeManagement
=========================================================================================================
This document will explains how repository created and project managed along with the detailed steps.

Task 1:
	Create repository with branches and provide pull permission to another user.
Task 2:
	Create versioning to Commit (Tagging)
=========================================================================================================


Step 1:
		Created Private Repository in GitHub name "EmployeeManagement"
		
Step 2: 
		Cloned this repository into my local repository
		git clone https://github.com/smadarapu01/EmployeeManagement.git
		
Step 3:
		Created Login.txt & EmployeeManagement.txt created in master 
		touch login.txt
		touch EmployeeManagement.txt
		git add .
		git commit -m 'some comments'

Step 4: 
		Pushing these change to remote repository "EmployeeManagement"
		git push origin master
		
Step 5:
		Created three branches 
			1. feature
			2. release
			3. hotfix
			4. master (default)
		e.g:
			git branch feature
Step 6: 
		Switched to release branch
		added release note for V1.0
		
		e.g: 
			git checkout release
Step 7: 			
		Switched back to master branch and merged with release branch
		
		e.g:
			git checkout master
			git merge release

Step 8:
		Switched to release branch 
		I felt this brach is stable to release so i will tag with version 1.0
		
		e.g:
			git tag -a V1.0 -m 'Stable version tagged with V1.0'
Step 9:
		Merged with master branch and pushed to remote repository "EmployeeManagement"
		
		e.g:
			git push origin release
Step 10:
		Pushed V1.0 tag to remote repository "EmployeeManagement"
		
		e.g:
		git push origin  V1.0 
		
Step 11:
		Switched to feature branch
		add a file feature.txt and added feature branch enhancements and commited.		
		 		
Step 12:
		Switched to master branch
		updated EmployeeManagement.txt with ManagePermissions method
		commited & push to remote repository "EmployeeManagement"

Step 13:
		Switched to feature branch and merge
		since feature branch has dependent file which is modified in master branch
		provided merge comments
		e.g:
			git merge master 

Step 14:
		Switched to hotfix branch and added issues.txt file to track customer issues.
		Since there are many changes happend in master which are dependent in hotfix brach.
		so I made rebase master in hotfix.
		e.g:
			touch issues.txt
			git add .
			git commit -m 'comments'
			git rebase master
			
		
			
		
		

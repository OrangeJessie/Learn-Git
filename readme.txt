Commands for git


mkdir name_of_your_file			# make a git repository
cd name_of_your_file
pwd					# used to know your path

git init					# init your git repository

git add name_of_your_file			# add your file to git repository
git commit -m "tips of this modify"		# add tips of modify

git status					# get current status
git diff					# get difference of the last version

git log					# show history
git log --pretty=oneline			# log parameter

git reset --hard HEAD^			# roll current version to previous version

git reflog					# show historical commands and version head

git diff HEAD -- name_of_your_file		# difference between file in your computer and in theh repository

git checkout -- file				# file in computer back to file added or committed
git reset HEAD name_of_your_file		# unstage file added to computer

git rm file_need_delect			# delect file in repository
git checkout -- file_need_restore		# restore delected file


git remote add origin https://github.com/OrangeJessie/Learn-Git.git		# local association with github

git push -u  origin master			# upload master to github, the first time use -u
git push origin master			# upload new version

git clone git@github.com:OrangeJessie/repository_name.git		# clone from github, make a repository offline

git remote				# show info in github
git remote -v				# more detail

git push origin master			# push local repository
git pull					# get new version from github
git branch --set-upstream-to <branch-name> origin/<branch-name>	# if cannot pull



git checkout -b dev				# make and switch to a new branck "dev"
git branch dev				# make a new branch
git checkout dev				# switch to this branch

git branch				# show all branch
git merge dev				# merge two branch
git merge --no-ff -m "tips" dev		# merge with no fast and make new commit
git branch -d dev				# deleted branch dev

git log --gragh --pretty=oneline --abbrev-commit			# show history


git stash					# store workplace
git stash list				# show all stash
git stash apply				# restore workplace in stash
git stash pop				# restore workplace in stash and delect stash

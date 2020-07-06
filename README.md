# Docs

# Clone Private Repo

> git clone git@github.com:username/repo.git

# Delete Local Branch

> git branch -d branch_name

OR

> git branch -D branch_name

# Fetch Remote Branches to Local

> git branch -r | grep -v '->' | while read remote; do git branch --track "${remote#origin/}" "$remote"; done

> git fetch --all

> git pull --all

# Reset Remote to certain Commit

> git reset --hard <>

> git push -f origin master

# Update Fork Master

> git remote add upstream git://github.com/

> git fetch upstream

> git merge upstream/master master

> git push

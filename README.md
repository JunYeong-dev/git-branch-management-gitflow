## Git flow tutorial for IntelliJ
* Create github repository in IntelliJ
```
1. VCS
2. Import into Version Control
3. Share Project on GitHub
4. OK
5. Add
```
* Start git flow
```
1. Open the IntelliJ terminal
2. C:\git-branch-management-gitflow>git flow init
3. Enter all
```
---
* Create local feature branch
```
1. Open the IntelliJ terminal
2. C:\git-branch-management-gitflow>git flow feature start first-feature
```
* Commit to local feature branch
```
1. Create any file
2. Open the IntelliJ terminal
3. C:\git-branch-management-gitflow>git commit -m "first commit"
```
* Merge local feature branch to local develop branch
```
1. Open the IntelliJ terminal
2. C:\git-branch-management-gitflow>git checkout develop
3. C:\git-branch-management-gitflow>git merge --no-ff feature/first-feature
```
* Delete local feature branch
```
1. Open the IntelliJ terminal
2. C:\git-branch-management-gitflow>git checkout feature/first-feature
3. C:\git-branch-management-gitflow>git flow feature finish first-feature
```
---
* Create local release branch
```
1. Open the IntelliJ terminal
2. C:\git-branch-management-gitflow>git flow release start "v1.0"
```
* Merge local release branch to local master branch
```
1. Open the IntelliJ terminal
2. C:\git-branch-management-gitflow>git checkout master
3. C:\git-branch-management-gitflow>git merge --no-ff release/v1.0
```
* Delete local release branch
```
1. Open the IntelliJ terminal
2. C:\git-branch-management-gitflow>git checkout release/v1.0
3. C:\git-branch-management-gitflow>git flow release finish -m "v1.0"
```
* Push local develop branch to origin develop branch
```
1. Open the IntelliJ terminal
2. C:\git-branch-management-gitflow>git checkout develop
3. C:\git-branch-management-gitflow>git push --set-upstream origin develop
```
* Push local master branch to origin master branch
```
1. Open the IntelliJ terminal
2. C:\git-branch-management-gitflow>git checkout master
3. C:\git-branch-management-gitflow>git push
```
---
* Create local hotfix branch
```
1. Open the IntelliJ terminal
2. C:\git-branch-management-gitflow>git flow hotfix start "v1.1"
```
* Commit to local hotfix branch
```
1. Create any file
2. Open the IntelliJ terminal
3. C:\git-branch-management-gitflow>git commit -a -m "hotfix/v1.1 commit"
```
* Merge local hotfix branch to local master branch
```
1. Open the IntelliJ terminal
2. C:\git-branch-management-gitflow>git checkout master
3. C:\git-branch-management-gitflow>git merge --no-ff hotfix/v1.1
```
* Delete local hotfix branch
```
1. Open the IntelliJ terminal
2. C:\git-branch-management-gitflow>git checkout hotfix/v1.1
3. C:\git-branch-management-gitflow>git flow hotfix finish -m "v1.1"
```
* Push local develop branch to origin develop branch
```
1. Open the IntelliJ terminal
2. C:\git-branch-management-gitflow>git checkout develop
3. C:\git-branch-management-gitflow>git push --set-upstream origin develop
```
* Push local master branch to origin master branch
```
1. Open the IntelliJ terminal
2. C:\git-branch-management-gitflow>git checkout master
3. C:\git-branch-management-gitflow>git push
```

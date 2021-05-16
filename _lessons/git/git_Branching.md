---
layout: mypage
heading : "You are being asked to work on an issue  “iss53” for your website project . While half way through it you received a request for a hotfix that needs to be done immediately. After fixing the hotfix you also need to return back to your iss53 issue. How to manage this using Git?"

vcode: 549543376
---
{: .table .table-striped}
 No. | Steps | Commands 
 1 |Go To directory. |cd Merge
2|Create a branch iss53|git branch iss53
3|Checkout the branch|git checkout iss53
4|Work on issue 53|touch issue53.html
5|Add the file  to staging area|git add issue53.html
6|Commit the file|git commit -m "Added issue53.html"
 7|Checkout master branch|git checkout master
8|Create a branch hotfix|git branch hotfix
9|Checkout the hotfix branch|git checkout hotfix
10|Fix the defect|touch hotfix.html
11|Add the file to staging area|git add hotfix.html
12|Commit the file|git commit -m “Fixed hotfix"
13|Checkout the master branch|git checkout master
14|Merge the hotfix branch|git merge hotfix
15|List the existing branches|git branch
16|Delete the hotfix branch|git branch -d hotfix
17|Checkout the iss53 branch and modify the file. Commit the file| git checkout iss53 vi issue53.html git commit -m “message”
18|Merge the branch and push the commit|git checkout master git merge iss53 git push


#### Sub Task
You have a master branch and a iss53 branch. You now need to merge the issue branch. How would you merge? 

{: .table .table-striped}
 No. | Steps | Commands 
 1 |Go to the folder Merge|cd Merge
2|List the branches. |git branch
3|Checkout master (Make sure you are on the master branch)| git checkout master
4|Merge iss53 branch |git merge iss53 -m "Recursive merge for iss53"
5|Push the commit| git push
6|Delete the iss53 branch| git branch -d iss53
7|List the branches| git branch





 

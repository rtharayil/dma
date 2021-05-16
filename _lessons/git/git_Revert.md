---
layout: mypage
heading : "While doing some defect fixes earlier you have ended up in a commit which is not relevant for you anymore. This commit was done earlier and all the commits after that is relevant.Also you want to keep the old commit in the history as for logging purpose . How would you solve it?"
vcode: 549543534
---
{: .table .table-striped}
 No. | Steps | Commands 
 1 |List the commits |git log --oneline
2|Select a commit and show the files that went into the commit |git show your_commit_Id
3 |Revert the selected commit| git revert your_commit_Id
4|List the commits |git log --oneline
5|Select the new commit and show the file changes |git show new__commit_Id


 

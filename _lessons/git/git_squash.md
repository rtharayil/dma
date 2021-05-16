---
layout: mypage
heading : While you were working for defect fix you have created multiple commits for a single defect and published it  . Your lead suggested you to squash these commits together into one commit.How would you solve the problem
vcode: 549146302
---
{: .table .table-striped}
 No. | Steps | Commands 
 1 |Get the status of the files |git status
2|List the commits |git log --oneline
3|Delete the last two commits |git reset --soft HEAD~2
4|List the commits|git log --oneline
5|Get the status of the files |git status
6|Create a new commit |git commit -m “<message>” 
7|Push the files forcefully|git push -f


 

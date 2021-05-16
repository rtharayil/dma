---
layout: mypage
heading : You have fixed an issue in your e-commerce application. But later it was identified that the issue was actually related to some configurations in your production servers and no actual code changes needs to be done. You need to remove the changes and commit done for the issue even from the commit history. How would you solve it?
vcode: 549146547
---
{: .table .table-striped}
 No. | Steps | Commands 
 1 |List the commits|git log --oneline
2|View the modifications done in the commit| git show commit_id
3|Delete the last commit|git reset --hard HEAD~1
4|List the commits|git log --oneline
5|View the file |cat contact.html


 

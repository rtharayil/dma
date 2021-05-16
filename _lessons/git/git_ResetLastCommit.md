---
layout: mypage
heading : "Assume that you are going to work on a defect say Issue No: 11 where we need to add email and mobile details to contact page of your e-commerce application. Accidentally we did a part of it and  staged it. But then we understood we had to add more details. So we again modified the file then committed the file. But all your modifications is not present in the commit. How would you solve it ?"
vcode: 549146408
---
{: .table .table-striped}
No. | Steps | Commands 
1|Go to folder ModifyingStagedFile|cd ModifyingStagedFile
2|Modify the file, contact.html (add Email)|vi contact.html
3|Add the file to staging area|git add contact.html
4|Modify the file again(add Mobile )|vi contact.html
5|Get the status of the file|git status|
6|Committed the file|git commit -m “message”
7 |View the modifications that went into the commit|git show commit ID
8|Get the status of the file|git status
9|Get the difference between working directory and last commit|git diff
7|Reset the last commit|git reset HEAD~1
8|Get the status of the file|git status
9|Add the files to staging area|git add .
10|Commit the file|git commit -m "Modified contact.html"


 

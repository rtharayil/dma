---
layout: mypage
heading : "Your application adds lot of logs while executing. Some of the logs that was created during your unit testing phase got added up to the source code repository. You are fed up with this and want to make sure that logs never even accidentally gets added to your repository. How would you set this up?"

vcode: 549543479
---
{: .table .table-striped}
 No. | Steps | Commands 
 1 |Go to directory gitignore |cd gitignore
2|List down the files in the path |ls
3 |Assume a new log file is created by your application|touch log0102.txt
4 |Check the status| git status
5 |Create a .gitignore file in the root path|vi .gitignore
6|Enter the file details to be ignored in the .gitignore file|  log*.txt  
7 |Check the status  |git status
8|Add .gitignore to staging area|git add .gitignore
9|Check the status  |git status
10 |Commit the file |git commit -m "Added .gitignore"


 

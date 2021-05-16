---
layout: mypage
heading : "As you do defect fixes you modified 3 files but file modifications in one file was not completed. But you added all 3 files to staging area so that it could be committed. How would you stop half done code from being committed?"

vcode: 549146243
---
{: .table .table-striped}
No. | Steps | Commands 
1 |Go to directory “RemoveFileFromStagingArea”|cd RemoveFileFromStagingArea
2|'Edit the files by bringing the files into editable format using “Esc” + “i” key pair. After editing save each files with the key combination “Esc” with “wq!”. Then press “enter”'|vi mango.html vi beans.html vi carrot.html
3|Add all files to staging area|git add .
4|Get the status of the file|git status
5|Remove mango.html from the staging area by the following command |git reset HEAD mango.html
6|Commit the remaining files|git commit -m " message "
7|Push the files|git push
8|Modify the third file “mango.html”|vi mango.html
9 |Commit |git commit -m " message "
10|push the file|git push


 

# Git guide for begginers:
**Version control**: It’s a system that helps you getting back to previous version of your files whenever you would like to do so, and it’s very helpful because through it you keep track of changes that you have previously made and comparing them as well.
Types of version control:
1.	**Local version control**: It involves one database on your hard disk that stores changes made on your files.
2.	**Centralized version control**: It involves a single server that stores all changes, modifications and file versions on it as it eliminates the usage of a local database also it can be accessed by many clients which helps team members keeping tracks of the changes made by other members.
3.	**Distributed version control**: This type of version control doesn’t solely depend on the server as it may crash and cause data loss, if the data isn’t backed up this could cause a huge problem for the team therefore this type has been created in order to allow clients to make repositories on their own pcs to back up data and avoid such problems.
The best example could be given about DVC’s is GIT and it is well-known for many reasons as it uses:
1.	**Snapshots**: Git is a DVC that stores data in the form of file systems and keeps snap shots of every time you make changes on your file by clicking on the button that says ‘’Commit changes’’ even if you don’t make changes it creates a reference to keep it backed up.
2.	**Local operations**: Git uses its local operations because all of the important data exists on its own local resources meaning you don’t need to fetch data from servers and also you can get the job done while offline.
3.	**Tracking changes**: it tracks all changes made and can detect problems that affects data easily.
4.	**Loss of data**: It is nearly impossible to loose snapshotted files on Git after committing changes.
5.	**States of file**: Your files on Git can only exist in three main states.
•	*Committed state*: Means the data is stored on a local database.
•	*Modified state*: Means changes have been made but you haven’t pressed commit yet.
•	*Staged state*: Means changes have been made and committed.

6.	**Graphical clients**: Git has its own GUI’s tools but you can make use of third party tools as it        allows.
7.	**Initial customization**: Git allows this through settings and by the doing the following steps: 
•	*Configuration of variables*.
•	*Identity settings*.

8.	**Default text editor**: In case you didn’t configure text editor then Git will use the systems default editor.
9.	**Check settings**: By using ‘’git config –list’’.
10.	**Getting help**: Git allows you to get more information’s about a specific command in three ways (‘git help command’, ‘git command –help’, ‘man git-command’).
11.	**Importing**: Through it you can import an existing project in your Git in various ways.
12.	**Cloning**: It creates a copy of your repository for different uses.
##Git workflow:
Local repository structure
![Local repository structure]( https://blog.udemy.com/wp-content/uploads/2015/08/image036.png)
Then we save changes.
##Life cycle of files
![Local repository structure]( https://blog.udemy.com/wp-content/uploads/2015/08/image006.png)

## A few file commands to know:
1.	***Check file***: Use ‘’git status’’.
2.	***Tracking and staging new files***: for a single file use ‘’git add filename’’ for all files use “git add *’’.
3.	***Committing a file***: Use ‘’git commit –m ‘’made change X, Y, Z’’’’.
4.	***Committing all changes***: Use ‘’git commit –a’’.
5.	***Pushing changes***: Use ‘’git push origin master’’.
6.	***Stash changes***: Use ‘’git stash’’.
7.	***Remote repositories***: Use ‘’git remote’’ or ‘’git remote –v’’ to view the full thing.
## For more in depth information’s check the following link:
[Local repository structure]( Git Tutorial: A Comprehensive Guide | Udemy Blog).

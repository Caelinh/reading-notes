# What is Git?

-**Snapshots**: Git is a DVCS(Distributed version control system) that stores data in a file system made up of snapshots. Each time you save a changed version of your project — called commit — Git creates a snapshot of the file and stores a reference to it.<br>
-**Local Operations**: Git relies on local operations because the most necessary information resides on the local disk. Eliminating the need to pull it from a server constantly.<br>
-**Tracking changes**:  Every change to a file is tracked and Git will inform what has changed and if anything has been corrupted.<br>
-**Loss of data**: Git makes it extremely difficult to accidently lose data. If it's commited your not gonna lose it.<br>
>Files in git have 3 main **states**.<br> 
>1.*Committed*: Data is securely stored in a local database.  
>2.*Modified*: Data is securely stored in a local database.  
>3.*Staged*: Flagged a file’s changed version to be committed in the next snapshot.

# Important Git Commands
> to add existing files from github to local machine >git clone 'url'  
> to see the source of your repo >git remote -v  
> current status of the git >git status  
>> **_important_** to add/update file >git add _filename_  
>> **_important_** to commit >git commit -m "_why your making the changes_"  
>> **_important_** to push local files to update github >git push origin main  
>> to pull github updates and update local files pull >git pull origin main  

_Make sure to commit changes frequently!!_

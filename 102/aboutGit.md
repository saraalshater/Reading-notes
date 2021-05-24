# **Git**

## **Before Git:**
### Imoprtant things to explain in order to understand Git
- **VCS**: *Version Control System, Allows you rectified mistakes  easily.*
  -  Local Version Control systems (CVCS). 
  - Centralized Version Control (DVCS): *This system entails a single server storing all changes and file versions, which can be accessed by various clients.*
  -  Distributed Version Control (DVCS): To prevent losing your folders.




## What is ***Git*** ?

Git is a DVCS that stores data in a file system made up of snapshots. Each time you save a changed version of your project — called commit — Git creates a snapshot of the file and stores a reference to it. If the file has not changed, Git only stores a reference to the already-stored identical version of it.

### **Git** :
1. Relies on local operations.
2. Git will always detect file corruption or loss of information in transit.
3. Git makes it extremely difficult for a snapshot of your file that is committed to be lost.
4. Files in Git can reside in three main states: committed, modified and staged.

### **Using Git**: 
This is some of the examples of using Git
* To customize you Git you should use `git config`

* To check settings, use the git `config --list` command.
* To get help use `git help command` note that there's other ways to get help. 
* Switch to the target project’s directory `cd test`
* To determine the state of files, utilize the `git status` command
* Track one file only by using the following format `git add filename`
* Track all files in a repository by using the following command `git add *`
* Committing a files `git commit -m “why you made it”`
* Committing all files `git commit -a`
* Pushing changes `git push origin main`
*When you are not ready to commit changes but do not want to lose them either use `git stash` 

### **Local Repository Structure**
1. Working Directory
2. Index
3. Head

### **The Life Cycle of File Status**
1. After you edit a file, Git flags it as modified because of changes made after the previous commit. 
2. You stage the modified file
3. Then, you commit staged changes.

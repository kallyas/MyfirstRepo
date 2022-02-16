 # Working with Git and Github

### Git commands
- <b>git init</b>
  will create a new local GIT repository. <br>
  The following Git command will create a repository in the current directory:<br>
  ```bash
  git init
  ```
  Alternatively, you can create a repository within a new directory by specifying the project name:
  ```bash
  git init [project name]
  ```
- <b>git clone<b>: is used to copy a repository. If the repository lies on a remote server, use:
  ```bash
  git clone https://github.com/kallyas/myfirstrepo.git
  ```

  - <b>git add</b>: is used to add files to the staging area. <br>For example, the basic Git following command will index the temp.txt file:
  ```bash
  git add <temp.txt>
  ```
  - <b>git commit</b>: will create a snapshot of the changes and save it to the git directory.
  ```bash
  git commit –m “Message to go with the commit here”
  ```
  > Note that any committed changes won’t make their way to the remote repository.
  
  - <b>git config</b> can be used to set user-specific configuration values like email, username, file format, and so on.
  <br>To illustrate, the command for setting up an email will look like this:
```bash
  git config --global user.email youremail@example.com
 ```
The –global flag tells GIT that you’re going to use that email for all local repositories. <br>If you want to use different emails for different repositories, use the command below:
 ```bash 
git config --local user.email youremail@example.com
 ```
  - <b>git status</b> displays the list of changed files together with the files that are yet to be staged or committed.
```bash
  git status
 ```
  - <b>git push</b> is used to send local commits to the master branch of the remote repository. Here’s the basic code structure:
```
  git push origin <master>
 ```
Replace `<master>` with the branch where you want to push your changes when you’re not intending to push to the master branch.

  - <b>git checkout</b>: creates branches and helps you to navigate between them. For example, </br>the following basic command creates a new branch and automatically switches you to it:
```bash
  command git checkout -b <branch-name>
To switch from one branch to another, simply use:
git checkout <branch-name>
 ```
  - <b>git remote</b>: lets you view all remote repositories. The following command will list all connections along with their URLs:
```bash
  git remote –v
 ```
To connect the local repository to a remote server, use the command below:
```bash
  git remote add origin <host-or-remoteURL>
 ```
 <br>
  
> Meanwhile, the following command will delete a connection to a specified remote repository:
 <br>
  
```bash
  git remote rm <name-of-the-repository>
 ```
  - <b>git branch</b>: will list, create, or delete branches. For instance, if you want to list all the branches present in the repository, the command should look like this:
```bash
  git branch
  ```
If you want to delete a branch, use:
```bash
  git branch –d <branch-name>
 ```
  - <b>git pull</b> merges all the changes present in the remote repository to the local working directory.
```bash
  git pull
 ```
  - <b>git merge</b> is used to merge a branch into the active one.
```bash
  git merge <branch-name>
 ```
  
- Features
- Chores
- Fixes

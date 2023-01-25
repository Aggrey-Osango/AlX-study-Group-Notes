### Forwading. #intro
This note is about git and github.
The note follows a youtube tutorial [Git and GitHub for Beginners - Crash Course](https://www.youtube.com/watch?v=RGOj5yH7evk) and I recomend watching the video. this note is to serve as a reference.

Introduction #concepts #terms 
	### 1. Version Control System: #T_Version_Control_System
		This is the management and tracking of changes in documents,computer procesess, website and other collection of information. GIT is one of VCS.
	### 2. Repository:
		A Folder where your project is saved, it can be on your local machine or hosted on a platform like github.

Git commands covered. (*all of the commands are in lowercase*)
	1. **git clone**  => This command copies a repository hosted somewhere else on your *local machine* (==computer==).
	2. **git add**    => adds a file or folder to be Tracked for changes in Git ("*changes are made on your local machines files*").
	3. **git commit** => Save your files on Git repository ("*either localy or online*").
	4. **git push**   => Uploads git commits to a remote repository hosting platform like github.
	5. **git pull**   => Download changes from a remote repository hosting platform to your local machine,("*opposite of push*").
	6. **git status** => shows all the files that were updated, created or deleted but have not been saved in a commit yet.
	7. **git init**   => Initialized a local folder to be a git repository("*Used when you created a local folder on your machine and want it to be a git repositoy*").
	8. **git remote add origin online-created-repo-addres** ("*used for linking locally created repo to the one on git hub*")
	9. git remote -v ("*used to show remote git repos that are linked to the current local repo*")
	10. **git branch**   => Show how many branch a repo has.
	11. **git checkout name-of-branch** => used to switch between branches ("*when used with the -b flag it creates a new branch from the master and switches to it*")
	12. **git diff name-of-branch**      => Show what is different in the current branch as compare to the main branch.

**NOTE:** For one to push changes to github you have to connect your local machine to github and prove that you are the owner of the project, this is done by generating an ==SSH KEY== that will be used for the connection.
```Example-Command-for-generating-SSH-Key
ssh-keygen -t rsa -b 4096 -C "email adress here"
```

*Complete SSH-KEY generation tutorial walk through* [Generating ssh key](https://www.youtube.com/redirect?event=video_description&redir_token=QUFFLUhqazJBLUhSX3diWW10d21lSDJVNWRtMGwwUHRiQXxBQ3Jtc0trc21hVXM5V2R5T2hFT0s0b3pmVTE5N1A1MWZiOHNPQk9OUG9aUlpjaDVudkMyQnBybXRNUmYyZWJqVmtaeWtXX2hfNlBSZmRtd3h4b1podmo1R2hqYTBjcF9qbmd2WVExb3ozeXYwcFo3SjJDa0tKMA&q=https%3A%2F%2Fhelp.github.com%2Fen%2Fgithub%2Fauthenticating-to-github%2Fgenerating-a-new-ssh-key-and-adding-it-to-the-ssh-agent&v=RGOj5yH7evk)

**Terminal Commands Covered**
	1. pbcopy => copies text to your clipboard ("*same as ctrl-c command from the keyboard*").
	2. 



> git push -u origin mster
 > 	This above command uses a *flag -u* to indicate direction of commit, *-u is means up stream*, when this is done, the subsequent push commands you can omit the source and destination argument.
 > 	* source       = origin = local-repo
 > 	* destinantion = master = online-repo
 > 

git remote add origin online-created-repo.

"The  above command uses a command known as ==remote== to mean that link the current local repo to the one in github that is empty so that you may push the commits to it."


## Work Flow Comparison.
#### GitHub Repo VS Local Repo
Click => [[Chat Comparison.canvas]]
	
### Git Branching.
#### Concepts of Branchin.
##### Types of branching 
* master/main/default
* feature
* hotfix

Braching is a technique where you turn your repo into a tree like structure so that you can servor and test different concepts and feature in your software. the way this works is that git allows you to split your code base of project into two non linked copy. you can make changes in one without interfering with the other and vice verser. The naming convetion is that the origian copy is called the main branch, and the unliked copy is feature branch. by default git uses master as a name for the original repo, this can be changed in config files to something like default, main e.t.c.

#### Uses of braching.
**Features:** This technique is used to test out new features in your software, without breaking the original code base.

**Test:** You may test new ideas and theories or even optimize your code.

**Fixbugs:** You can use branching to fix an error or a bug that was found. braching is a good way of ensuring code integrity.

### Misllenious:
git push origin master:
	This is used when you have cloned a repo from git, otherwise
	
	
	
	
	
	
	
	it will give you an error.
	For this command to work when you haven't cloned the repo is to create an empty repo on git and connect the local folder to it.
    Example-of-linking.
    git remote add origin newly_created_empty_repo_address.




Questions: #quiz
	1. What is the difference between ==git push== and ==git push==
	2. Is it necesarry to create the repo on my local machine when I have to create another one online then link it?
	3. Is there a way of making my local git project master without first having to create it online?
	4. Can one split a repo then remerge them in the future?
	5. Is it possible to work on two code base from a single branch and merge them in the future?
# Introduction
## What is Git and GitHub?
### Git: 
Version control, also known as source control, is the practice of tracking and managing changes to software code over time.  [**Git**](https://git-scm.com/about) is a distributed version control software and is the most commonly used version control system. A Git repository tracks and saves the history of all changes made to the files in a Git project. It saves this data in a directory called .git, also known as the repository folder. Git tracks the changes you make to files, so you have a record of what has been done, and you can revert to specific versions should you ever need to. Being distributed means that every developer working with a Git repository has a copy of that entire repository - every commit, every branch, every file. Git also makes collaboration easier, allowing changes by multiple people to all be merged into one source.  

So, regardless of whether you write code that only you will see, or work on as part of a team, Git will be useful for you. In some cases it may even be a required skill for a test team.

Git is software that runs **locally**. You normally use Terminal (MacOs) or Git Bash (Windows) and use git commands to manage the local repository and eventually push your changes to a remote repository in order to collaborate with others. Your files and their history are stored on your computer until you push them to a remote repository. Unlike other VCS software (i.e. CVS, Subversion, Perforce) you do not need to have an internet connection to do some work. You can work locally and eventually upload to remote repository when you have a internet connection.   

But wait, if Git is run locally how can everyone be making changes? What do you mean by push to a remote repository? That is were GitHub comes in.


### GitHub:
GitHub is a for-profit company that offers a cloud-based Git repository hosting service. Essentially, it makes it a lot easier for individuals and teams to use Git for version control and collaboration. So, while Git is storing your code locally, GitHub is where you can store your code remotely and share with others. It's important to remember that GitHub is **_not_** Git. There are other companies who offer hosting services that do the same thing as GitHub, such as Bitbucket and GitLab, but GitHub is by far the most widely used, with over 100 million developers. It is even possible to have your own remote repository server, but it is much easer to use one of these services. 

GitHub’s interface is user-friendly enough so even novice coders can take advantage of Git. Without GitHub, using Git generally requires a bit more technical savvy and use of the command line.

### Git Stages:
The following is important — here is the main thing to remember if you want the understand how to work with Git. Git has three main states that your files can reside in: modified, staged, and committed:

- Modified means that you have changed the file but have not committed it to your database yet.
- Staged means that you have marked a modified file in its current version to go into your next commit snapshot.
- Committed means that the data is safely stored in your local database.

This leads us to the three main sections of a Git project: the working tree, the staging area, and the Git directory.

 <img src="/images/GitStages.jpg" width="50%" height="50%">
 
The working tree is a single checkout of one version of the project. These files are pulled out of the compressed database in the Git directory and placed on disk for you to use or modify.

The staging area is a file, generally contained in your Git directory, that stores information about what will go into your next commit. Its technical name in Git parlance is the “index”, but the phrase “staging area” works just as well.

The Git directory is where Git stores the metadata and object database for your project. This is the most important part of Git, and it is what is copied when you clone a repository from another computer.

The basic Git workflow goes something like this:
1. You modify files in your working tree.
2. You selectively stage just those changes you want to be part of your next commit, which adds only those changes to the staging area.
3. You do a commit, which takes the files as they are in the staging area and stores that snapshot permanently to your Git directory.

If a particular version of a file is in the Git directory, it’s considered committed. If it has been modified and was added to the staging area, it is staged. And if it was changed since it was checked out but has not been staged, it is modified. Please refer to [Git documentation](https://git-scm.com/book/en/v2/Getting-Started-What-is-Git%3F) for deeper dive.

### GitHub Workflow:
What does the work flow look like? Each circle represents a commit or change in the software. The green is the master or main source code that will most likely be hosted remotely (i.e. GitHub). The blue and orange are branches of the main branch. Branches allow you to develop features, fix bugs, or safely experiment with new ideas in a contained area of your repository. Notice that you can have other branches of the code that can eventually merge into the main branch. Branches allow the "main" branch to be the deployable working code.   

<img src="/images/git-branches-merge.png" width="50%" height="50%">


## [Next - Step 2: Getting Started](2_GetStarted.md)

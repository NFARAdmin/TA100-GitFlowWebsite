# Working in a Team:  

Congratulations! You created a repository and have an idea of the steps to stage, commit, and push your changes. Don't worry, you will get some more practice later on.  

Now that you've pushed some of your code to your remote repository are your ready for something slightly different. Have you worked with others on the same repository? Ahh, that can be interesting. One of the many benefits of Git is that it allows many developers to work on the same repo at once. There is a process for doing that. While there may be slight differences between organizations, they follow these general steps:

<!-- 1. --> 
   - #### Step 1. Clone or fork repository
   - #### Step 2. Create a branch in your repository
   - #### Step 3. Make changes to your branch.
   - #### Step 4. Stage changes, Commit changes, and push your changes to remote branch
   - #### Step 5. Create a pull request
   - #### Step 6. Address review comments
   - #### Step 7. Merge your pull request
   - #### Step 8. Delete your branch
 
## To clone or to fork, that is the question..... ?
Any **public** Git repository can be forked or cloned. A *fork* creates a completely independent copy of Git repository. In contrast to a fork, a Git *clone* creates a ***linked*** copy that will continue to synchronize with the target repository. 

<img src="images/git_clone_vs_fork.jpg" width="70%" height="70%">

When a Git repository is cloned, the target repository remains shared amongst all of the developers who had previously contributed to it. Other developers who previously contributed to that codebase will continue to push their changes and pull updates from the cloned repository. Any developer who clones a repository can synchronize their copy of the codebase with any updates made by fellow developers.

In contrast to a clone, a Git fork operation will create a completely new copy of the target repository. The developer who performs the fork will have complete control over the newly copied codebase. Developers who contributed to the Git repository that was forked will have no knowledge of the newly forked repo. Previous contributors will have no means with which they can contribute to or synchronize with the Git fork unless the developer who performed the fork operation provides access to them.

When a repository is forked, developers who plan to work with the new codebase (i.e. the forked codebase) will still need to perform a git clone operation on the forked repository. You'll still need to run push and pull operations to synchronize local changes with the forked repo, as shown in the diagram below. However, changes and updates to the forked repository will be isolated to the fork and will not be reflected in the original repo.



### Thanks for the explanation, so which one should I do? 
If you would like to make changes directly to a repository you have the **permission** to contribute to, then cloning will be the first step. You can clone ANY public repository, but you may not be able to contribute to it. 

If you don’t have permissions to contribute to the repository, but would like to experiment with the repo, a fork is the way to go. If you want, afterwards, you can create a pull request to submit your changes to the original repository.

## What’s the difference between a Pull and a Push?
The difference between a “pull” and a “push” is as intuitive as you think. The git *pull* command is used to fetch and download content from a remote repository and immediately update the local repository to match the content. A *push* is not a request, but a **command** (git push) used to “upload” local content or changes to a remote repository. Many of you may have been *pushing* your code to your own repository. 

## What is a pull-request:
A pull request is an event to notify software developers that a team member has pushed code to a specific Git branch (or a specific version of the code repository) for a colleague to review. Once a developer opens a pull request, your team can review the potential changes introduced before merging with the central repository branch. 

## The Anatomy of a Good Pull Request 
Whenever a developer opens a pull request, they should be sure to include all of the following components: 
<!-- 1. --> 
   - ### The Title
      - The title should be a meaningful summary of the purpose of the PR. Often this can correspond to a ticket, service, or component. 

   - ### The Description
      - The description should include changes the developer introduced so the reviewer knows what to look out for. 

   - ### Commits
      - Each relevant commit should be included in your PR and each commit should have a concise description of code changes. 

Now that you have an idea of the work flow, let's get the remote repository on your local drive. 

### [Next - Step 5: Clone Repository](5_CloneWebsite.md)

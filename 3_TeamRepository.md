# Working in a Team:  

Congratulations! Now you have an idea of what Git and GitHub are, and you have installed both of them as well. Maybe you've even pushed some of your code to your remote repository. But, have you worked with others on the same code? Ahh, that can be interesting. One of the many benefits of Git is that it allows many developers to work on the same code at once. There is a process for doing that. While there may be slight differences between organizations, they follow these general steps:

<!-- 1. --> 
   - #### Step 1. Clone or fork repository
   - #### Step 2. Create a branch in your repository
   - #### Step 3. Make changes to your branch. Commit, and push your changes
   - #### Step 4. Create a pull request
   - #### Step 5. Address review comments
   - #### Step 6. Merge your pull request
   - #### Step 7. Delete your branch
 
## To clone or to fork, that is the question..... ?
Any public Git repository can be forked or cloned. A *fork* creates a completely independent copy of Git repository. In contrast to a fork, a Git *clone* creates a ***linked*** copy that will continue to synchronize with the target repository. 

When a Git repository is cloned, the target repository remains shared amongst all of the developers who had previously contributed to it. Other developers who previously contributed to that codebase will continue to push their changes and pull updates from the cloned repository. Any developer who clones a repository can synchronize their copy of the codebase with any updates made by fellow developers.

In contrast to a clone, a Git fork operation will create a completely new copy of the target repository. The developer who performs the fork will have complete control over the newly copied codebase. Developers who contributed to the Git repository that was forked will have no knowledge of the newly forked repo. Previous contributors will have no means with which they can contribute to or synchronize with the Git fork unless the developer who performed the fork operation provides access to them.

When a repository is forked, developers who plan to work with the new codebase (i.e. the forked codebase) will still need to perform a git clone operation on the forked repository. You'll still need to run push and pull operations to synchronize local changes with the forked repo, as shown in the diagram below. However, changes and updates to the forked repository will be isolated to the fork and will not be reflected in the original repo.

<img src="images/git_clone_vs_fork.jpg" width="70%" height="70%">

### Thanks for the explanation, so which one should I do? 
If you would like to make changes directly to a repository you have the **permission** to contribute to, then cloning will be the first step before we implement the actual changes and push.

If you don’t have permissions to contribute to the repository, but would like to implement changes anyway, a fork is the way to go. If you want, afterwards, you can create a pull request to integrate your changes to the original repository.

## What’s the difference between a Pull and a Push?
The difference between a “pull” and a “push” is as intuitive as you think. A developer will *pull* to request a target repository to pick up their local changes and merge them into the existing code. A *push* is not a request, but a **command** (git push) used to “upload” local content or changes to a remote repository. Many of you have been *pushing* your code to your own repository. 

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

### [Next - Step 4: Clone Repository](4_CloneWebsite.md)

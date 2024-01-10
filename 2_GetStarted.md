# Some Setup Required
Before we we will need to introduce you terminal and setup git on your workstation. 

## Intro to Terminal
All of the Git commands run in Terminal. What is Terminal? The Mac Terminal is a command line interface (CLI) for the MacOS operating system (OS) that lets you communicate with the operating system. You enter commands and scripts (called shell scripts) to perform tasks on your Mac. Percy Grunwald from TopTechSkills has an excellent 15min video about Terminal for beginners. Please take a moment to view the [video](https://www.youtube.com/watch?v=aKRYQsKR46I) and familiarize yourself with Terminal then come back here. If interested in learning more on your own time, a more in depth explanation can be found [here](https://www.youtube.com/watch?v=ogWoUU2DXBU). 

While there are many graphical user interface (GUI) based softwares that can run git commands on your repository, it is very important to learn the git commands for Terminal. For one, the command line is the only place you can run all Git commands — most of the GUIs implement only a subset of Git functionality for simplicity. If you know how to run the command-line version, you can probably also figure out how to run the GUI version, while the opposite is not necessarily true. Also, while your choice of graphical client is a matter of personal taste, all users will have the command-line tools installed and available on their workstations.

Here is how you access terminal:

1. Press the Command key + Spacebar on the keyboard to open [Spotlight](https://support.apple.com/guide/mac-help/search-with-spotlight-mchlp1008/mac). For windows keyboards the **Windows** key is used in place of the Command key.  When you do this the Spotlight Search bar will appear:

<img src="images/spotlight.png" width="50%" height="50%">

2. Enter the word "Terminal" in the spotlight search and select Terminal from the list. A Terminal window will open:

<img src="images/terminalwindow.png" width="40%" height="40%">

3. When you open terminal it will open in the home directory by default. The home directory is the logged-in users working folder. You know you are in the home directory when you see the following :
   
```
 userName@ComputerName ~ %
```    
The ~ (tilde) indicates you are in the home directory. 

Here are some useful commands for terminal (% is prompt and not part of the command):

```
- To see the path of your current directory (Print Working Directory):
% pwd
- To list content of current directory (List items):
% ls
- To navigate to a folder enter folder name after cd (you don't include <around the name>, this is just an example): 
% cd <folder_Name>
- To navigate back up one folder:
% cd ..
- To navigate back up two folders:
% cd ../..
- To navigate to the root folder:
% cd /
- To navigate to the home folder:
% cd ~
- To clear the screen (just leave a prompt):
% clear
- To create a file (you must enter the file extension):
% touch <filename.html>
- To create a folder (Make Directory):
% mkdir <folderName>
- To remove/delete a file:
% rm <index.html>
- To remove/delete an empty folder:
% rmdir <folderName>
- To remove/delete a folder and all of its contents use the "-r" flag (be very careful, this can't be undone):
% rm -r <folderName>
- To copy a file (must be in the folder you want to copy into, expressed as ./ at the end):
% cp <filepath/fileName> ./
Example: copy "index.html" file from "webcourse" folder into your current folder:
% cp webcourse/index.html ./
- To copy an empty folder (must be in the folder you want to copy into, expressed as ./ at the end):
% cp <folderName> ./
- To copy a folder and all of the contents use the -r "flag" (must be in the folder you want to copy into, expressed as ./ at the end):
% cp -r <folderName> ./
Example: copy "webcourse" folder into your current folder and all of its contents you use the "-r" flag:
% cp -r webcourse ./
- To include a space in folder or file name include a \ and then include the space (try to avoid using spaces in file and folder names):
The following will create a folder named "new folder"
% mkdir new\ folder
The following will create a file named "index ten.html"
% touch index\ ten.html
You must also use the backslash to access the directory:
The following will acccess the folder with the name "new folder"
% cd new\ folder
```
Please note that you want to refrain from using spaces when creating file/folder names. We only talk about it here in case you encounter it. Each project will have certain rules around naming conventions. The most common [naming conventions](https://www.freecodecamp.org/news/programming-naming-conventions-explained/) are camel case (camelCase), snake case (snake_case), kebab case (kebab-case), or pascal case (PascalCase). During our course we will be using camel case. 

Please note that there are also [keyboard shortcuts](https://support.apple.com/guide/terminal/keyboard-shortcuts-trmlshtcts/2.14/mac/14.0) for Terminal that you might find useful. 

## Remote Repository 
Can you use Git without a remote repository account? Yes, but then your repository will only be available locally and not available to others. You want to push your repository to a remote repository in order to collaborate with others. During this course we will be using GitHub; remember their are other services out there. Remember, *Git* is local, *GitHub* is for remote repositories. 

Do you have a GitHub account? If you do, great, if not, please create one here [GitHub Sign Up](https://github.com/signup?ref_cta=Sign+up&ref_loc=header+logged+out&ref_page=%2F&source=header-home). Make sure to use your **personal** email when creating the GitHub account. You will eventually use this account to store your work and possiblky use on your resume. A couple of things about your GitHub account:
   - Make sure to use two factor authentication when creating your account.
   - Write down your GitHub username, password, and email for future use. You will need this for password recovery. 
   - Email your GitHub username to your technical instructor.

After creating your GitHub account we will come back here.  

## Do you have Git installed?
Now that you have been introduced to Terminal and have a GitHub account let us get going with Git. Since we will be working with Macs, all steps are for MacOS. Most MacOS computers have Git pre-installed you just have to get it activated. If you want to work from home you have to take a couple more steps (more details later). 

1. Open Terminal. Since you will be working on shared computer lets make sure to create folder for all of your work. While in this home directory create a folder with your name (first initial and Last Name). If your name is "Wallace Grommet" the folder name will be "wGrommet". Enter the following command:

```
mkdir <firstinitialLastname>
```
You just created a folder. All of your work will go in this folder. Every time you open terminal you will navigate to this folder before starting your work. 

2. Navigate to your folder by entering the following command:

```
% cd <yourName>
```
3. Make sure to confirm that you have Git installed. You can do this by running the following git command in Terminal:
```
% git --version
```
Terminal will output something like this:
```
% git version 2.39.2
```

Not installed? Here is a guide on how to install Git on your computer: [Install Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git). Follow the steps in order to install Git (make sure to follow steps for your operating system - MacOS or Windows ). 

4. Once you have Git installed we need to customize the environment:

From the Terminal command prompt let's make sure to set up your identity by setting your user name and email address. This is important because every Git commit uses this information, and it’s immutably baked into the commits you start creating. In Terminal enter the following (enter **your** information inside the quotation marks): 
```
% git config --global user.name "your-github-user-name"
% git config --global user.email "your@email.com"
```

If you want to check your configuration settings enter the following command in Terminal:

```
git config --list
````
This command will list all the settings Git can find at that point (yours will look different):
```
$ git config --list
user.name=John Doe
user.email=johndoe@example.com
color.status=auto
color.branch=auto
color.interactive=auto
color.diff=auto
```
There are a lot of Git commands and you are not expected to know them all. You can always use a reference for the [Git commands](https://git-scm.com/book/en/v2/Appendix-C%3A-Git-Commands-Setup-and-Config) or download one of the following cheat sheets: 
[GitHub Education Git Commands Cheat Sheet](images/git-cheat-sheet-education.pdf) or [GitLab Git Commands Cheat Sheet](images/images/git-cheat-sheet.pdf)



## [Next - Step 3: Working in a Team](3_TeamRepository.md)

# Creating a GitHub Repository and Connecting it to Your Xcode Project

## Step 1: Create a GitHub Repository

1. Name it whatever you want
2. Initialize the respository with a README 
3. Add a .gitignore with a tag of "Swift"

![](https://github.com/znpierucci/DigitalConceptTutorial/blob/master/images/Step1.png "Step 1")


## Step 2: Edit .gitignore

When dealing with Swift, every project has .DS_Store files that must be ignored, which is why we put ".DS_Store" in the ".gitignore" file.

1. Open your .gitignore file and click the pencil to edit it
2. Type ".DS_Store" on line 24 of the .gitignore file
3. Commit the file

![](https://github.com/znpierucci/DigitalConceptTutorial/blob/master/images/Step2.png "Step 2")

## Step 3: Locate Your Xcode Project Folder

If you have not already created an Xcode project, [click here to learn how](https://github.com/znpierucci/DigitalConceptTutorial/blob/master/XcodeTutorial.md).

My Project folder is found in my desktop:

![](https://github.com/znpierucci/DigitalConceptTutorial/blob/master/images/Step3.png "Step 3")

## Step 4: Open Terminal

If you do not know where the Terminal program is, do the following

1. Press Command + SpaceBar
2. Type in "Terminal"
3. Click the Terminal Program that looks like the following

![](https://github.com/znpierucci/DigitalConceptTutorial/blob/master/images/Step4.png "Step 4")

## Step 5: Locate Your Project Directory Using Terminal

To change directories, you must type in "cd" followed by the name of the folder or location you are looking to change into.

For example, if you would like to switch to your desktop, you must type in "cd Desktop"

To change into your project folder, locate the path of the project folder, and cd into the location, then cd into the project folder.

For example, if your project folder is on your desktop, do the following:

1. Type "cd Desktop" and press enter
2. Type "cd HelloWorldExample" (or whatever your project is named) and press enter
3. Type "ls" and press enter to see all of your files

You are now inside your Project Directory!

![](https://github.com/znpierucci/DigitalConceptTutorial/blob/master/images/Step5.png "Step 5")

## Step 6: Connect GitHub to your Project

1. Type the following commands in order in Terminal
>git init

>git add .

>git commit -m "First commit"


![](https://github.com/znpierucci/DigitalConceptTutorial/blob/master/images/Step6.png "Step 6")

2. Copy the url of your GitHub repository by clicking the green "Clone or download" button on your repository home page and then clicking the clipboard symbol to copy it to your clipboard
![](https://github.com/znpierucci/DigitalConceptTutorial/blob/master/images/CopyURL.png "Copy URL")
3. Type the following command in terminal, replacing the word "url" with the URL of your GitHub repository
>git remote add origin url 
4. Type the following commands in order in Terminal
>git pull --rebase origin master

>git rm -r --cached .

>git add .

>git commit -m "Applied .gitignore"

>git push -u origin master

![](https://github.com/znpierucci/DigitalConceptTutorial/blob/master/images/Step6p2.png "Step 6")

Your project is now connected to GitHub!

Reload your repository to check it out.
Your repository should now have all of the project files in it, rather than just the README.md and .gitignore

![](https://github.com/znpierucci/DigitalConceptTutorial/blob/master/images/Step6p3.png "Step 6")


# Congratulations! Your Swift Project now has a GitHub Repository!



## Extra Step: Committing Your Project Without Having to Use Terminal Again

Lets say your current project looks like this: 

![](https://github.com/znpierucci/DigitalConceptTutorial/blob/master/images/commit1.png "Step 1")

If you type some code, your online GitHub repository will not update. You have to manually commit and push your progress for it to show up on your online repository.

For example, if you type in some code on a project that has an online GitHub repository connected to it, there will be blue bars next to all of the lines of code that have been changed, to give the programmer a sense of what has been changed since the last commit. 

![](https://github.com/znpierucci/DigitalConceptTutorial/blob/master/images/commit2.png "Step 2")

If you want to commit these changes to your online repository, click "Source Control" in the top menu bar of Xcode.

![](https://github.com/znpierucci/DigitalConceptTutorial/blob/master/images/commit3.png "Step 3")

Click "Commit..." to commit these changes, and the following window should pop up:

![](https://github.com/znpierucci/DigitalConceptTutorial/blob/master/images/commit4.png "Step 4")

Type in your commit message, which can be whatever you would like it to be, then make sure to check the "Push to remote" box if you would like it to automatically push to a certain branch. 

>Note: For this example, I am pushing to my "Master" branch becuase it is a small project with no other branches, but it is good practice to create different "Feature" branches, push your progress to those branches, then push those to master, rather than straight to master.

Once those steps are done, click "Commit # File(s) and Push" button (this button will be different depending on how many files were modified) and then it will commit all of your changes to your online GitHub repository.

![](https://github.com/znpierucci/DigitalConceptTutorial/blob/master/images/commit5.png "Step 5")

# Complete!

[Click here to go back to the main page](https://github.com/znpierucci/DigitalConceptTutorial/blob/master/README.md)

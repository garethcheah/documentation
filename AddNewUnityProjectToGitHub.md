# How To Add New Unity Project to GitHub

The following is based on the use of Sourcetree as a visual client to GitHub.

## 1. Create new Unity project through Unity Hub

## 2. Ensure project settings are correct for version control

  There are two important settings that your Unity project needs to have before you use it with git:
  - Version Control Mode set to Visible Meta Files
  - Asset Serialization Mode set to Force Text

  In modern versions of Unity, these settings are the default, but it is worth checking them if your project originated in an older version of Unity.

## 3. Initialize the project for Git

  - Open Terminal window via Sourcetree
  - Browse to your project folder
  - Run 'git init' to add git conifiguration to your project

## 4. Add a new repository

  - In Sourcetree, select 'Add'
  - Set 'Working Copy Path' to your project folder. After initialization in step 3, this should now be recognized as a Git repository
  - Ensure the name of the project is to your liking
  - Keep 'Local Folder' option as '[Root]'
  - Click on 'Add' button.

## 5. Add .gitignore file

  - Create a new file with your text editor
  - Paste in the contents of the gitignore template for Unity from:
    - [Local template](.gitignore)
    - [Unity template provided by GitHub](https://github.com/github/gitignore/blob/master/Unity.gitignore)
  - Save it as '.gitignore' in the root of your project directory

## 6. Commit project files to GitHub

  - In SourceTree, you should now see your project workspace with a bunch of uncommitted changes. Select 'uncommitted changes'.
  - Under 'Unstaged files', you should see files within your project folder (minus files that were excluded by .gitignore)
  - Press the 'Stage All' button
  - Press the 'Commit' button
  - Now you are ready to perform your first commit into your new GitHub repository

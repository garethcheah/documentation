# How To Add New Unity Project to GitHub

The following is based on the use of Sourcetree as a visual client to GitHub.

## 1. Create new Unity project through Unity Hub

## 2. Create new repository in Sourcetree

  - Open Sourcetree
  - Select option to 'Create' new repository
  - Under 'Destination Path', browse to your Unity project folder
  - Ensure the name of the repo is to your liking
  - Ensure repo type is 'Git'
  - Leave 'Create Repository On Account' unchecked to just create the repo locally for now.

## 3. Create .gitignore file for Unity project (this step can also be done when creating a repo on GitHub.com)

  - Within your local repo in Sourcetree, open 'Settings'
  - Switch to advanced tab. Under 'Repository-specific ignore list', click on the 'Edit' button. This should open up a new .gitignore file in a text editor.
  - Paste in the contents of the gitignore template for Unity from:
    - [Local template](.gitignore)
    - [Unity template provided by GitHub](https://github.com/github/gitignore/blob/master/Unity.gitignore)
  - Save file
  - Go back to Sourcetree and click 'OK' to close 'Repository Settings' window

## 4. Create initial commit to local repository

  - Within your local repo in Sourcetree, you should now see a bunch of unstaged files. Click on 'Stage All' button.
  - Click on the 'Commit' button.
  - Enter a description for the commit and click on the 'Commit' button
  - You should now see your first commit in the 'master' branch

## 5. Create remote respository in GitHub.com

  - Go to github.com and sign into your account
  - Create a new remote repository with the same name matching the local repository for your project
  - After the remote repository is created, copy the URL for the new repository

## 6. Add path to remote repository in Sourcetree

  - Go back to your local repo view in Sourcetree and click on 'Settings'
  - Under the 'Remotes' tab, select the option to 'Add' a remote repository path
  - For 'Remote name', check the box for 'Default remote'
  - For 'URL / Path', paste the URL copied in step 5
  - Ensure you select your GitHub account under 'Remote Account'
  - Click on 'OK' button

## 7. Push changes committed to local repository to remote repository

  - Back in your local repo view, click on the 'Push' button
  - Check the box beside your 'master' local branch, and ensure that the 'master' remote branch is also selected
  - Click on 'Push'
  - If no errors appear, then your local commits should now be in your remote repository as well. You can also go to your repo at github.com to verify this. You should be able to see all your project files and commits.

## 8. DONE

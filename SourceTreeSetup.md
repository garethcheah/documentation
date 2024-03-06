# How To Setup Sourcetree

## 1. Download and install Sourcetree

  - https://www.sourcetreeapp.com/

## 2. To get Sourcetree to connect with GitHub using SSH, first you must generate a SSH Key (see instructions below for how to do this on Windows PC)

  - Open Command Prompt
  - Generate SSH Key by typing 'ssh-keygen' and press Enter. This will generate 2 files representing your rsa key pair: one public and one private with file extension of .ssh. 
  - Next you'll be prompted to enter a paraphrase (password)
  - After this, you can confirm that the key generation is successful by browsing to your user folder. You should see a '/.ssh' folder containing 2 files typically named 'id_rsa'
  - Online resource: https://www.howtogeek.com/762863/how-to-generate-ssh-keys-in-windows-10-and-windows-11/

## 3. Add SSH key to GitHub

  - Assuming you already have an account setup with GitHub, log into GitHub and go to Settings under your profile
  - Click on the 'SSH and GPG keys' under the Access heading the the left nav
  - Press on the 'New SSH key' button. Here is where you will add the key that you generated in the previous step
  - Open the public id_rsa.pub file and copy its content
  - Go back to GitHub, and paste the content into the 'Key' textbox
  - Give your key a unique name in the 'Title' textbox
  - Press the 'Add SSH key' button

## 4. Configure SSH key in Sourcetree

  - Open up the Sourcetree app that was previously installed in step 1
  - Go to Tools > Options to open the Options dialog box
  - Under 'SSH Client Configuration', specify the location of your 'id_rsa' file
  - In the 'SSH Client' drop-down, select OpenSSH
  - Click on the 'OK' button to save the new configuration
  - Online resource: https://stackoverflow.com/questions/56980052/how-to-configure-ssh-keys-on-windows-for-sourcetree-terminal-and-ides-such-as-i

## 5. DONE

  - For a good video tutorial on using Git for Unity with Sourcetree, watch this: https://www.youtube.com/watch?v=DgFWpSKyT7I&t=165s
  - Another good resource of how to set up a Unity project in GitHub: https://unityatscale.com/unity-version-control-guide/how-to-setup-unity-project-on-github/

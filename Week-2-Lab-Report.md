The first step about how to log into a course-specific account on ieng6 is to install VScode. To do this search up VSCode in your browser and click on the download.

![VSCode Download](VSCodeDownloadPage.PNG)

On this website you should click the download button for your operating system and install VSCode.

The next step to logging into a course-specific account is to install OpenSSH.

To install open SSH you should open settings > Apps > Apps and Features > Optional Features. 
Once you are here you should make sure you have OpenSSH installed and if you do not find and install OpenSSH client and OpenSSH server.

After you have OpenSSH go to look up your course-specific CSE15L account and create your password.
After you have set up your account and password you can log into your account in VSCode.

Once you are in VSCode you can type the command ssh `cse15lwi22aqe@ieng6.ucsd.edu` except `aqe` will be replaced by letters in your course-specific account
Then enter your password to login into the remote server.

![Logging into Remote Server](VSCode%20ssh%20login.PNG)

Once you have logged in you can test out some commands.

![Commands](lab1Part4.PNG)

Here we test the cd command which should not print anything and the ls command which lists some files.

Once you have tried testing some commands you can create a file and add some code.
Then you can upload the file to the remote server with the `scp` command and run your code.

![scp command](lab1Part5.PNG)

As we can see in the picture when we run ls the file WhereAmI.java has been uploaded to the remote server and can be run.

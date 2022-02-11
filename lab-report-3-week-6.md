# Week 4 Lab Report

## Streamlining ssh Configuration

## .ssh/config file

![Config file](CreatingTheFile.PNG)

To make the config file we needed a basic file rather than a txt file so our group just copied the id_ed25519 file and renamed it to config and changed its contents.

![In file](SettingUpConfig.PNG)

The contents of this file were edited on Notepad and were copied straight from the lab instructinos. Then we changed the user to cs15lwi22aqe which is my course specific remote server username.

## SSH command logging in

![SSH Login](SSHConfig.PNG)

Here I log into ssh using the `ssh ieng6` command. ieng6 is alias I saved in the config file.

## Using SCP command with Streamline

![Using SCP to copy files](StreamlineSCP.PNG)

Here I am able to use the command `scp MarkdownParse.java ieng6` because of the streamline configuration. If I did not have the configuration I would have to type out all of `cs15lwi22zz@ieng6.ucsd.edu`

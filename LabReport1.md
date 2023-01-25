# CSE 15L WI 23 Lab Report 1
## 1. Meet your group
Groups will be divided into 6-8 people and will be overseen by a discussion leader. This will be dependent on your seat and for this week's lab, you are free to choose your seat along with your group. Once these groups are formed, open the google doc corresponding to your group number, make sure that it's the right time period along with the right location.

Discuss and write down the answers to the questions below in the google doc.
  - What is your name (you can include anything else anyone might want to know like pronouns or a nickname)?
  - What is your major?
  - Pick one of these three to answer for the next one:
    - What is a UCSD club or organization that you're in or interested in?
    - What is your favorite spot on campus so far?
    - What is a little shortcut or trick that you know about UCSD?

## 2. Your CSE15L Account
The link below redirect you to find your CSE15L account and from there, reset your password according to the instructions given.
- Click the link [here](https://sdacs.ucsd.edu/~icc/index.php)

Follow these steps if you need any help in resetting your password.
  1. Once you've opened the link, go to the area where it says account lookup and enter in your student ID and your UCSD username and click submit, after this step you'll obtain your account ID for this class. (it should be similar to cs15lwi23abc)
  2. Click on that account ID and it will direct to another page where near the top of the page, there will be a hyperlink to change your password.
  3. Enter in your current password and your new password where it tells you to. If don't you want this password to also be changed for your tritonlink password, make sure you change the __"Change my Tritonlink Password"__ to no.
  4.  Don't click check password, instead go back to the password confirmation box and click on it, then press enter.
  5.  It could take up to 15 minutes for the password reset to go through the system so be patient, but if it doesn't take that long then go ahead and move onto the next step.
  6.  Try to type in the command below and then enter in your password, as you type it in nothing will show up, but that's perfectly normal. (the "$" should not be in the command, it is jsut there to be recognized that it is a command, remember this for the next step)
- `$ ssh ACCOUNT_NAME@ieng6.ucsd.edu`

## 3. VS Code
Download [VS Code](https://code.visualstudio.com/) for your respective operating system and install it properly according to the instructions. 
- Once completed, open it up and it should look a little something like this, I already have it downloaded since I have used it for another class so don't worry about the files that I have there, but it should still look similar with maybe some different colors

![Imgur](https://i.imgur.com/NWrOE8p.png)


## 4. Remote Connection
If you're on windows, you'll have to do some of the next steps, but if it's not your operating system then you can just skip the next two steps.
1. Install [Git](https://gitforwindows.org/)
2. Once installed, open installed, open the terminal as __git bash__ in Visual Studio Code

If you're on Mac, just make sure that your terminal is set to bash

![Imgur](https://i.imgur.com/jdwjKiv.png)

Once accomplished, type in the command below switching out the "abc" for your account letters
- `$ ssh cs15lwi23abc@ieng6.ucsd.edu`

If it is your first time connecting to the server you'll probably get this message

```
- ⤇ ssh cs15lwi23abc@ieng6.ucsd.edu
  The authenticity of host 'ieng6.ucsd.edu (128.54.70.227)' can't be established.
  RSA key fingerprint is SHA256:ksruYwhnYH+sySHnHAtLUHngrPEyZTDl/1x99wUQcec.
  Are you sure you want to continue connecting (yes/no/[fingerprint])?
```

Type in yes and then you'll be prompted to type in your password, you're password won't be appearing that it is begin typed in, but is. Once you're connected you should see something similar to the picture below

![Imgur](https://i.imgur.com/KzJTZNn.png)

## 5. Run Some Commands
Once you're able to log into the system, try running some of the commands that have been used in class from using both the remote computer and your own personal computer. Report what you see and if there are any differences between any outputs of the operating systems.

Some commands you can try are:
* cd ~
* cd
* ls -lat
* ls -a
* ls/home/linux/ieng6/cs15lwi23/cs15lwi23xyz where xyz will be replaced with a repspective 15L account ID
* cp /home/linux/ieng6/cs15lwi23/public/hello.txt ~/
* cat /home/linux/ieng6/cs15lwi23/public/hello.txt

An example of this will look like this

![Imgur](https://i.imgur.com/m3LEfrs.png)

Just as a reminder, `cd` stands for change directory and the tilde (~) mark means home directory. The command `ls` stands for list which will list everything in the directory that you're in, but if you specify another directory by `-(directory name)` within the directory you're currently in or you can write an absolute path after the command to list out the files or directory in whatever directory you would like. The command `cp` is used to add a path to the class path in order to find the class file needed. The command `cat` will print out the file that you indicate it to.

Once Finished with this step you can exit the terminal doing the following steps:
* Press __Crtl + D__
* Type in the command prompt __exit__

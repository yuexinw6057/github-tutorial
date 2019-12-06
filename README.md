# GitHub Tutorial

<b> <i> By </b> </i> <i>Kayla Weng </i>

---
## Git vs. GitHub
<p6> Hello there reader, do you know what is the difference between git and github?
If not, you have came to the right spot. At first, I was confused too, but it is really not that hard.
<i> What is git? </i> You may ask:
Git is the system that creates mostly all the contents on github, allowing changes and edits onto the website.
There are also commands under the name of "git" some examples consists of:
git init, git add, git commit. <i> speaking of git init, let's go to our next point of git init. </i> </p6>
---
## Initial Setup
<p> To set up ur git or as we call it the "Ide" aka your workspace, you will need to do a set of commands (first to last, in order):
<ul>
    <li> git config --global user.email "you@example.com" (However, you need to use your email. Use HSTAT if you are from HSTAT. Also use quotes!) </li>
    <li> ssh-keygen -t rsa -b 4096 -C "you@example.com" then slowly press ENTER repeatedly until you got something like a square with random
    letters and numbers around it </li>
    <li> eval "$(ssh-agent -s)" </li>
    <li> After that, type: ls -al ~/.ssh <br /> you should see a file name that is id_rsa.pub </li>
    <li> Next, do: cat ~/.ssh/id_rsa.pub <br />
    copy all of the result to your clipboard (it should start with ssh-rsa and end with your email address)</li>
    <li> <b> YOU ARE ALMOST THERE! </b> You will soon go to: <br />
    https://github.com/settings/keys > New SSH Key > Title: ide50
Key: paste your ssh key
Press the green Add SSH key button </li>
    <li> Go Back in your cs50 IDE, do sudo nano ~/.ssh/config <br />
    After you do that paste this:
    Host github.com
    Hostname ssh.github.com
    Port 443 <br /> control+X to exit, then press Y then ENTER </li>
    <li> Further more, type: ssh -T git@github.com </li>
    <li> lastly, Type yes, press ENTER. <i> All Done! </i>

<p3> To start an intial setup in order for github and git to work together, you would have to first use a git command call: <br />
<i> </i> git init <br />
However, before that you will need a directory, what is a directory? Read Workflow and Commands to understand more of the commands that is
needed to create an amazing beginner website!</p3>

<p> Now at this point, you may ask yourself: <i> What exactly does git init do? </i> <br />
The command git init makes a brand new repository. Which in plain english meaning that nothing is in there, think of it as a empty clean box.
It initializes git. </p>

---
## Repository Setup
<p> hello, you are here still, I assume you are very interested in how to do it now. So let's begin.
SO first, you will need to start up with the repository at <i> <a href= "github.com"> Github.com </a> </i> <br />
Afterwards, you will need to click on the downward error in order to see a drop down menu, that way you will see something that says
"repositories." After finding that, you click on it and it should say "new" in a green button, when you see that, you click on it.
Afterwards, you will see your username and a box where it says "new repo name" (repo is shortened for repository), after you named it, you will
scroll down and press create repository, meaning that a space for website is completed and ready to use. <br />
<p> Now after you do that, you should go back to your ide.cs50.io and create a directory using mkdir "insert name you want your directory to be"
then you will cd into the file (more on that on the next section).
You will now be doing the folling steps to set up your repo:
<ul>
    <li> after going into the directory you just created, you will use: git remote add origin git@github.com:"your username" </li>
    <li> then, git push -u origin master </ul>
    <li> which then soon you can start editing the file and making it appear on the website! </li>
</ul>
    To do that, continue on reading!</p>

---
## Workflow & Commands
<p4> If you have set everything up correctly, you should be at a very good place right now. So literally all your commands will execute.
If you your command isn't working properly, there is either something wrong with:
<ul>
    <li> The spelling </li>
    <li> Your ssh key (first ever ide set up) </li>
    <li> The directory you are in </li>
<ul>
</p4>
<p4> Back to what I was saying, now you have it set up with no problems (hopefully), you will now learn the commands from the expert! Aka me! (JK) <br />
Okay so basically, in order for you to actually put something onto a website, you must do the following commands (usually):
<ul>
    <li> <code> pwd - Check the working directories that you are at, the last one (read left to right) is the directory you are at </code> </li>
    <li> <code> cd .. or cd ../.. - change directory to the directory you want. Each two dot represents a level in the directory. To go to one,
    simply do cd "name of directory" </code> </li>
    <li> <code> Git init - initalizes git to branch master </code> </li>
    <li> <code> git add - adds the file you are working on to a staging area </code> </li>
    <li> <code> git commit -m "" - sounds like what it means, it means to commit it and basically put in something </code> </li>
    <li> <code> git push - allows it to be on github peacefully. </code> </li>
    <li> <code> git log - allows you to see what commits you have done </code> </li>
    <li> <code> git status - to see if there is any files that is left unadded or committed.  </code> </li>
    <li> <code> c9 - to open file when you are in the file's directory </code> </li>
</ul> </p4>
<p style="color:peach;"> Honestly there is more, but for now that is all you need to know. The end! Have a good one! </p>

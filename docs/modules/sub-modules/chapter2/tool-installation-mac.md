# Mac Install Guide

In this class, you can expect to be exposed to a wide range of tools with names you may have never heard. At first, the sheer number of tools you'll be expected to use may seem overwhelming but trust us! With a little time and a little effort, they will be as familiar to you as a scalpel is to a surgeon or a sewing needle is to a seamstress.

### Overview

In this assignment, you will be installing all the required tools and software necessary for the class. We've got a lot to install so buckle in and get ready!

### Before You Begin

Make sure you sign up for the below services. you'll need all of them throughout the course.

* GitHub: [https://github.com](https://github.com/)
* Slack: [https://slack.com/](https://slack.com/)

Also, make sure to accept the invite for your section on [Slack](https://slack.com/) as well. You will receive the link to your class-specific channel during orientation.

### Tool Installation

The rest of this assignment will walk you through the specific steps associated with installing each of the tools you'll need. Follow the instructions closely!

#### Google Chrome

1. If you don’t already have Chrome installed, visit the download page [here](https://www.google.com/chrome/browser/desktop/index.html).
2. Download, open, and run the installation file.

#### Zoom

#### Slack

You’ll be messaging your instructor, your TAs and your fellow classmates with this business-centric chatting app. The teaching and career staff will post some of their most important announcements here so set this program up as soon as you can. You will receive the link to your class-specific channel during orientation.

1. If you don’t have the Slack app yet, search for Slack in your Mac’s App store and then click the Get button under the app’s listing. Click the button again when it displays “install.”

    <p align="center">
         <img src="https://raw.githubusercontent.com/coding-boot-camp/enterprise-prework-assets/master/assets/Install-Slack.png" width="600" title="Slack">
    </p>

   * When the app finishes installing, open it and move on to step 2.

2. If you already use the Slack app, you just need to add our channel to your application.

   * Click the header of your current Slack Channel.
    <p align="center">
         <img src="https://raw.githubusercontent.com/coding-boot-camp/enterprise-prework-assets/master/assets/Install-Slack2.png" width="250" title="Slack2">
    </p>

   * Then, select “Sign in to another team …”

    <p align="center">
         <img src="https://raw.githubusercontent.com/coding-boot-camp/enterprise-prework-assets/master/assets/Install-Slack2.1.png" width="250" title="Slack2.1">
    </p>

3. As you run through the guide, make sure you do the following:

   * Enter in the domain we gave you for Slack.

    <p align="center">
         <img src="https://raw.githubusercontent.com/coding-boot-camp/enterprise-prework-assets/master/assets/Install-Slack3.1.png" width="250" title="Slack3.1">
    </p>

   * Enter in the email with which we invited you, as well as your password, when prompted.

    <p align="center">
         <img src="https://raw.githubusercontent.com/coding-boot-camp/enterprise-prework-assets/master/assets/Install-Slack3.2.png" width="250" title="Slack3.2">
    </p>

#### Terminal

You’ll be entering your command line code through this interface. Since you’re on a Mac right now, you already have it! Just follow these steps to open the program.

1. Press `command+space bar` to open Spotlight Search.

    <p align="center">
         <img src="https://raw.githubusercontent.com/coding-boot-camp/enterprise-prework-assets/master/assets/Install-Terminal-1.png" width="400" title="Terminal-1">
    </p>

2. Type “Terminal” into the search and then hit enter.

    <p align="center">
         <img src="https://raw.githubusercontent.com/coding-boot-camp/enterprise-prework-assets/master/assets/Install-Terminal-2.png" width="600" title="Terminal-2">
    </p>

3. Keep this window open. You’ll need it for the next steps.

    <p align="center">
         <img src="https://raw.githubusercontent.com/coding-boot-camp/enterprise-prework-assets/master/assets/Install-Terminal-3.png" width="600" title="Terminal-3">
    </p>

#### Java SDK

To install the Java SDK, watch this video, or follow the directions below.

<p align="center">
  <a href="https://youtu.be/9Bw8vpjYRiA" target="_blank"><img src="https://raw.githubusercontent.com/coding-boot-camp/enterprise-prework-assets/master/assets/jdk-thumb.png" width='400px'></a>
</p>

1. Head over to the [JDK download page](https://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html)

2. Accept the license agreement under the *Java SE Development Kit* box.

3. Click on the Mac OS X x64 download option.

4. In your browser, open the installation files package once the download is complete.

5. When the installation package window pops up, double click the package icon to launch the install wizard.

5. In the Introduction section of the install wizard, click "continue."

6. The Destination Select section should automatically choose an installation location and redirect you to the next section. 

7. Click "Install" in the Installation Type section.

8. Enter your password in the pop up prompt, and click "Install Software.".

9. Once the Installation section completes, you should see a message that says "The software was successfully installed." 

10. You will be automatically directed to the Summary Section, which means you've successfully installed Java.

11. Click the close button, and select "Move to Trash" for the installation files. 

12. Open Terminal and run the command "java -version" to check that the install completed successfully!

#### Eclipse

#### Selenium IDE

#### SSH Key

Generating SSH keys allows developers to interface with certain remote services without having to constantly type out login information. You're going to set up an SSH key for GitHub.

Without a key, you won’t be able to push your code to GitHub without entering a password each time. Trust us, that would be as irritating as needing a key to open every door in your home.

This handy video can walk you through the below steps:

<p align="center">
  <a href="https://youtu.be/Ajbf6WY3HgM" target="_blank"><img src="https://raw.githubusercontent.com/coding-boot-camp/enterprise-prework-assets/master/assets/Capture.JPG" width='400px'></a>
</p>

1. Sign up for an account on [https://github.com](https://github.com/).

2. Open up Terminal.

3. We need to set up SSH keys. First, let’s make sure you don’t already have a set of keys on your computer. Type this into your Terminal window\(copying and pasting will not work\):

   * `ls –al ~/.ssh`

   * If no keys pop up, move on to step 4.

   * If keys do pop up, check that none of them are listed under `id_rsa`, like in this image:

    <p align="center">
         <img src="https://raw.githubusercontent.com/coding-boot-camp/enterprise-prework-assets/master/assets/Install-SSHKey1.png" width="600" title="SSHKey1">
    </p>

   * If you do find a key with a matching name, then you can either overwrite it by following steps 4 to 6 or you can use the same key in steps 10 and beyond. Be advised that you'll have to remember the password tied to your key if you decide not to overwrite it.

4. Type in this command along with your email to generate your keys:

   * `ssh-keygen –t rsa –b 4096 –C "YOURGITHUBEMAIL@PLACEHOLDER.NET"`

5. When asked to enter a file to save the key, just hit the return key.

   * Also enter a passphrase for your key.

   * Note: You shouldn’t see any characters appear in the window while typing the password.

6. When you’re finished your window should look like this:

    <p align="center">
         <img src="https://raw.githubusercontent.com/coding-boot-camp/enterprise-prework-assets/master/assets/Install-SSHKey2.png" width="600" title="SSHKey2">
    </p>

7. For the next step, we need to use a tool called an SSH Agent. Let’s test whether that’s working on your machine. Run this command in Terminal:

   * `eval "$(ssh-agent –s)"`

   * If your Terminal window looks like the image below, move onto the next step.

    <p align="center">
         <img src="https://raw.githubusercontent.com/coding-boot-camp/enterprise-prework-assets/master/assets/Install-SSHKey3.png" width="600" title="SSHKey3">
    </p>

8. Now run this command:

   * `ssh-add ~/.ssh/id_rsa`

9. When prompted for a passphrase, enter the one associated with the key.

   * If you’ve forgotten this key, just go through step 4 to create a new one.

10. We need to add the key to GitHub. Copy the key to your clipboard by entering this command:

    * `pbcopy < ~/.ssh/id_rsa.pub`

    * You shouldn’t see any kind of message when you run this command. If you do, make sure you entered it correctly.

    * Do not copy anything else until you finish the next steps. Otherwise, you’ll have to enter the copy command again.

11. Go to [https://GitHub.com/settings/ssh](https://github.com/settings/ssh). Click the “New SSH key" button.

    <p align="center">
         <img src="https://raw.githubusercontent.com/coding-boot-camp/enterprise-prework-assets/master/assets/Install-SSHKey4.png" width="600" title="SSHKey4">
    </p>

12. When the form pops up, enter a name for your computer in the Title input. In the Key input, paste the SSH key you copied in Step 10.

    <p align="center">
         <img src="https://raw.githubusercontent.com/coding-boot-camp/enterprise-prework-assets/master/assets/Install-SSHKey5.png" width="600" title="SSHKey5">
    </p>

13. Now we just need to add GitHub to your computer’s list of acceptable SSH hosts. Go back to your Terminal window. Type in this command: `ssh –T git@github.com`

    * You should see an RSA fingerprint in your window. Only enter “yes” If it matches the one highlighted in the image below:

    <p align="center">
         <img src="https://raw.githubusercontent.com/coding-boot-camp/enterprise-prework-assets/master/assets/Install-SSHKey6.png" width="600" title="SSHKey6">
    </p>

#### Setting your Git username for every repository on your computer

Git uses a username to associate commits with an identity. The Git username is not the same as your GitHub username.

You can change the name that is associated with your Git commits using the `git config` command. The new name you set will be visible in any future commits you push to GitHub from the command line. If you'd like to keep your real name private, you can use any text as your Git username. Changing the name associated with your Git commits using `git config` will only affect future commits and will not change the name used for past commits.
    <p align="center">
         <img src="https://raw.githubusercontent.com/coding-boot-camp/enterprise-prework-assets/master/assets/Mod5-45.png" width="600" title="Mod5-45">
    </p>

#### Setting your email address for every repository on your computer

GitHub uses the email address set in your local Git configuration to associate commits pushed from the command line with your GitHub account.

You can use the `git config` command to change the email address you associate with your Git commits. The new email address you set will be visible in any future commits you push to GitHub from the command line. Any commits you made prior to changing your commit email address are still associated with your previous email address.

For more information on commit email addresses, including your GitHub-provided `noreply` email address, see "[About commit email addresses](https://help.github.com/articles/about-commit-email-addresses/)."
    <p align="center">
         <img src="https://raw.githubusercontent.com/coding-boot-camp/enterprise-prework-assets/master/assets/Mod5-46.png" width="600" title="Mod5-46">
    </p>

### Amazing!

If you got through all the installations, give yourself a pat on the back! Installations are never fun, but just like taxes, ya gotta do them.

Be sure to take a break before continuing with the rest of the pre-work.

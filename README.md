# Design Team
Design Team Sandbox including Tools, Tricks, Gists, Markdowns, etc.

>#### Important Note:
> If you haven't done so, please create a new github account with your username ending with "**-pmap**", e.g., "jsmith-pmap", so we can invite you to collaborate in our repositories. 


## Basic Software Configuration
The list below consists of the essential software apps, plugins and command line packages our team members get when joining the Product Design group at ProcessMAP.

We encourage you to install the following by yourself - just follow the list - so you get familiar with what the tools you will have at your disposal.

# Command Line Accelerators

## 1. Install Xcode
Xcode is Apple's development environment for creating apps. Download it from:
[http://developer.apple.com/xcode](http://developer.apple.com/xcode)

	You must agree to the license by opening Xcode.app before proceeding.

The next set of commands and applications will require the use of `Terminal`. Install the Command Line Tools from Xcode:

	xcode-select --install

## 2. Homebrew - Package Manager
Homebrew [http://brew.sh](http://brew.sh) is a package management system that simplifies the installation of software on the Mac OS X operating system.  

Homebrew will make the installation process easier. 

Open `Terminal` and enter the following command:

    ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)" 

- Press ENTER to continue.
- Enter System Password (your login password) 
- After installation is complete, be sure to run the following command:
    
    `brew doctor`

Wait for the message: `Your system is ready to brew.` and you are good to start **installing Git**.


## 3. Git - Source Control
Git is a distributed version control and source code management (SCM) system with an emphasis on speed. Now that you’ve got Homebrew installed, use it to install Git from within your `Terminal` by entering the following command line:

	brew install git

The Git installation is straightforward, but to confirm, test the install with the following command, to check Git's version:

	git version

## 4. Node.Js - Low-level Server Platform
Node.js is a software platform that is used to build scalable network applications. Node.js utilizes JavaScript as its scripting language, and achieves high throughput via non-blocking I/O and a single-threaded event loop.

Once again, Homebrew makes it easy to install the latest stable version for Node.js. Simply enter the following:

	brew install node

This should take about 4 minutes. Confirm the installation by checking Node latest version:

	node -v

And the great news is that Node Package Management (NPM) is also installed. Previous versions you had to install `npm` separately. Test it out:

	npm -v

Let me explain a bit about NPM if you are not familiar.

>### Important Note About NPM
NPM is a NodeJS package manager. As its name would imply, you can use it to install node programs. Also, if you use it in development, it makes it easier to specify and link dependencies.

>I strongly encourage you not to do package management with sudo! Packages can run arbitrary scripts, which makes sudoing a package manager command as safe as a chainsaw-haircut. Sure, it's fast and definitely going to cut through any obstacles, but you might actually want that obstacle to stay there.

>I recommend doing this once instead:

>	`sudo chown -R $USER /usr/local`

> That sets your user account as the owner of the /usr/local directory, so that you can just issue normal commands in there. Then you won't ever have to use sudo when you install node or issue npm commands.


## 5. Bower - The Package Manager for the Web
Bower [http://bower.io](http://bower.io) is a package manager for the web. It offers a generic, unopinionated solution to the problem of front-end package management, while exposing the package dependency model via an API that can be consumed by a more opinionated build stack. There are no system wide dependencies, no dependencies are shared between different apps, and the dependency tree is flat.

Bower is THE Package Manager to have if you want to manage installation dependencies for web development components, like AngulaJs, jQuery, etc.

Install Bower through `npm` as follows:

	sudo npm install -g bower
    
## 6. Web Font Load 

- Easily install ALL of [Google's Web Fonts](https://www.google.com/fonts) using the command line below. Learn more about this command on [qrpike's GitHub](https://github.com/qrpike/Web-Font-Load) in your terminal:

	curl https://raw.githubusercontent.com/qrpike/Web-Font-Load/master/install.sh | sh

---

# Desktop Applications


###  Apps
- [Sketch App](http://bohemiancoding.com/sketch/) by Bohemian Coding
 - [Learn Sketch](http://bohemiancoding.com/sketch/learn/)
 - [design+code overview on Sketch](https://designcode.io/sketch)
 - [Useful Sketch Links](http://bohemiancoding.com/sketch/community/)
- [Adobe Creative Cloud](http://www.adobe.com)
- Google Helpers:
 - [Google Chrome Canary](https://www.google.com/chrome/browser/canary.html)
 - [Chrome App Launcher](https://chrome.google.com/webstore/launcher)
 - [Google Drive](https://www.google.com/drive/download/)
- [Brackets](http://brackets.io/) - Code editor with live browser preview and updates without a server (requires Chrome) 
- [Git](https://git-scm.com/) - for designers ;-)
 - [Learn git](http://try.github.com/)
- [GitHub for Mac](https://desktop.github.com/) - Git client for those not fond of the command line geekness.
- [The Unarchiver](https://itunes.apple.com/us/app/the-unarchiver/id425424353?mt=12)


#### Apps Under Evaluation
Expecting team recommendations, please [post your suggestions here](https://github.com/ProcessMAP/Design-Team/issues)

- [Slack](https://slack.com/) - a badass chat platform for internal team communications
 - [9 Slack Hacks We Couldn't Live Without](https://keen.io/blog/105456820166/9-slack-hacks-we-couldnt-live-without)
 - [13 cool things you might not know you can do with Slack](http://thenextweb.com/apps/2015/02/05/13-cool-things-might-not-know-can-slack/)
 - [17 Slack integrations to spice up your team communication](http://wpcurve.com/slack-integrations/)

###  Browser Plugins
Expecting team recommendations, please [post your suggestions here](https://github.com/ProcessMAP/Design-Team/issues)

###  Prototyping Tools
Expecting team recommendations, please [post your suggestions here](https://github.com/ProcessMAP/Design-Team/issues)

---
#### Not the End... more to come for sure.

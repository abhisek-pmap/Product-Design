# Design Team
Design Team Sandbox including Tools, Tricks, Gists, Markdowns, etc.
These are the directions for setting up the dev environment for those who are using **Windows-based computers**.

>#### Important Note:
> If you haven't done so, please create a new GitHub account with your username ending with "**-pmap**", e.g., "jsmith-pmap", so we can invite you to collaborate in our repositories.


## Basic Software Configuration
The list below consists of the essential software apps, plugins and command line packages our team members get when joining the Product Design group at ProcessMAP.

We encourage you to install the following by yourself - just follow the list - so you get familiar with what the tools you will have at your disposal.

# Command Line Accelerators

## 1. PowerShell and Scoop - Command Line Installer & Task Automation for Windows

* Make sure you have PowerShell 3 installed first by going to  [here](http://www.microsoft.com/en-us/download/details.aspx?id=34595). Then, open Windows PowerShell and enter the following command to update the execution policy **(Note: Do NOT do this on servers)**:

```
	set-executionpolicy unrestricted -s cu
```

* Scoop [http://scoop.sh/](http://scoop.sh/) is a package management system that simplifies the installation of software on the Windows operating system. Install Scoop by entering the following command.

```
	iex (new-object net.webclient).downloadstring('https://get.scoop.sh')
```

- Press ENTER to continue. 
- Enter System Password (your login password).
- After installation is complete, be sure to run the following command:

```
	scoop install 7zip coreutils curl git grep openssh sed wget vim grep
```

## 2. Git - Source Control
Git is a distributed version control and source code management (SCM) system with an emphasis on speed.
You can install Git by typing in `scoop install git` in Windows PowerShell, or you can install Git for Windows [here](https://git-scm.com/download/win).

  - In Select Components, check Additional Icons, Windows Explorer Integration, and Associate .git* configuration files with the default text editor and associate .sh files to be run with Bash.
    - Press Next for Start Menu folder (it is automatically set to 'Git' by default unless you want to specify otherwise).
  - Adjusting your PATH environment
    - Select "Use Git from the Windows Command Prompt"
  - Configuring the line-ending conversions
    - Checkout Windows-style, commit Unix-style line endings
  - Configuring the terminal emulator to use with Git Bash
    - Use MinTTY (the default terminal of MSys2)

* Ensure that Git is installed by running the following in the command line.
	 `git version`

### Git links:

- [Learning Git and GitHub](https://help.github.com/articles/good-resources-for-learning-git-and-github/)

## 3. Node.Js - Low-level Server Platform
Node.js is a software platform that is used to build scalable network applications. Node.js utilizes JavaScript as its scripting language, and achieves high throughput via non-blocking I/O and a single-threaded event loop.

You can install Node.js by typing in `scoop install node` in Windows PowerShell, or you can download the latest version of node for Windows [here](https://nodejs.org/en/) and install v4.2.1 LTS (Long-Term Support). 

Run the installer (the .msi file that you downloaded from the Node.js site) and follow the prompts in the installer. Accept the license agreement, click the 'Next' button several times and accept the default installation settings. Restart your computer.

**Test Node** - Confirm the installation by checking the latest version of Node in the command line:
```
	node -v 
```
which should print a version number, so you'll see something similar to `v4.2.1`.

**Test NPM** - Node Package Management (NPM) is also installed with Node. Check the latest version of NPM by typing in the following in the command line:
```
	npm -v 
```
which should print a version number, so you'll see something similar to `v2.14.7`.

>### Important Note About NPM
NPM is a NodeJS package manager. As its name would imply, you can use it to install node programs. Also, if you use it in development, it makes it easier to specify and link dependencies.

>I strongly encourage you not to do package management with sudo! Packages can run arbitrary scripts, which makes sudoing a package manager command as safe as a chainsaw-haircut. Sure, it's fast and definitely going to cut through any obstacles, but you might actually want that obstacle to stay there.

>I recommend doing this once instead:

>	`sudo chown -R $USER /usr/local`

> That sets your user account as the owner of the /usr/local directory, so that you can just issue normal commands in there. Then you won't ever have to use sudo when you install node or issue npm commands.

##### Read more about updating Node and NPM [here](http://blog.teamtreehouse.com/install-node-js-npm-windows).

## 5. Gulp - JavaScript Task Runner

Gulp is a JS task runner that lets you automate tasks such as:
- Bundling and minifying libraries and stylesheets
- Less/Sass to CSS compilation
- Refreshing your browser when you save a file
- Quickly running unit tests and running code analysis
- Copying modified files to an output directory

Type in the following into the command line:
```
	npm install -g gulp
```

The **-g** is an _optional_ flag used to signify that we want to install this package globally so that any project can use it. Check the command line to ensure that there are no error messages. Type in the following in the command line:
```
	gulp -v
```

You should see something similar to `CLI version 3.9.0` and `Local version 3.9.0`.


## 6. Bower - The Package Manager for the Web
Bower [http://bower.io](http://bower.io) is a package manager for the web. It offers a generic, unopinionated solution to the problem of front-end package management, while exposing the package dependency model via an API that can be consumed by a more opinionated build stack. There are no system wide dependencies, no dependencies are shared between different apps, and the dependency tree is flat.

Bower is THE Package Manager to have if you want to manage installation dependencies for web development components, like AngulaJs, jQuery, etc.

Install Bower through `npm` as follows:

	sudo npm install -g bower

## 7. Sass - Stylesheet Language

In order to install Sass (a Ruby gem), you need to first install Ruby on Windows [here](http://rubyinstaller.org/).

Download **Ruby 2.2.3** and press 'I agree' for the License Agreement. 

**When going through the installation wizard, select only the middle option to 'Add Ruby executables to your PATH'**. Otherwise, you will get an error message stating that Ruby is not recognized as an internal or external command when you try to install Sass in the command prompt.

Open up the command prompt (cmd) and type in the following:
```
	gem install sass
```
Hit Enter/Return and wait for Sass to be installed.

Ensure that Sass is installed by running the following in the command line: 
```
	sass -v
```

You should see something similar to `Sass 3.4.19 (Selective Steve)`.


---

# Desktop Applications

### Text Editor
- [Atom Text Editor](https://atom.io/) is a modern text editor that works across operating systems, has a built-in package manager, and helps you write code faster with smart autocompletion.

#### Atom Text Editor Packages (optional but highly recommended)
- [Atom Beautify](https://atom.io/packages/atom-beautify) - Cleans up the formatting of HTML, CSS, JavaScript, etc. code in Atom.

- [Linter](https://atom.io/packages/linter) - Allows you to easily visualize errors and other messages.

- [Linter Tidy](https://atom.io/packages/linter-tidy) - Will 'lint' your `.html` opened files in Atom.

- CSS Color Pickers
	- [Web Box Color](https://atom.io/packages/webbox-color) - Simple CSS color viewer.
	- [Color Picker](https://atom.io/packages/color-picker) - Another color viewer; reads HEX, RGB, RGBa, among others and is able to convert between formats.

- Git
	- [Git Blame](https://atom.io/packages/git-blame) - Annotations for files.
	- [Git Context](https://atom.io/packages/tualo-git-context) - Adds basic Git commands to the file tree menu.
	- [Git History](https://atom.io/packages/git-history) - View previous versions of any file known to Git.
	- [Git Log](https://atom.io/packages/git-log) - Shows a graph of your Git commits and other commit related information.

- [Terminal Panel](https://atom.io/packages/terminal-panel) - Executes your commands and displays the output.
	- Install httpster (simple local static development server) `npm install -g httpster`
	- Choose the port `$ httpster -p (number here, e.g. 8800)`
	- Reload Atom and enable LiveReload on Chrome Browser

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

- [Principle](http://principleformac.com) - Principle makes it easy to create animated and interactive user interface designs. Whether you're designing the flow of a multi-screen app, or new interactions and animations, Principle lets you create designs that look and feel amazing.
- [Slack](https://slack.com/) - a badass chat platform for internal team communications
 - [9 Slack Hacks We Couldn't Live Without](https://keen.io/blog/105456820166/9-slack-hacks-we-couldnt-live-without)
 - [13 cool things you might not know you can do with Slack](http://thenextweb.com/apps/2015/02/05/13-cool-things-might-not-know-can-slack/)
 - [17 Slack integrations to spice up your team communication](http://wpcurve.com/slack-integrations/)

###  Browser Plugins
Expecting team recommendations, please [post your suggestions here](https://github.com/ProcessMAP/Design-Team/issues)

- Google Chrome
	- [Full Page Screen Capture](https://chrome.google.com/webstore/detail/full-page-screen-capture/fdpohaocaechififmbbbbbknoalclacl?utm_source=chrome-ntp-icon) - Takes a full page screen capture of your current browser window.
	- [LiveReload](https://chrome.google.com/webstore/detail/livereload/jnihajbhpnppcggbcgedagnkighmdlei?utm_source=chrome-ntp-icon) - Provides browser integration for LiveReload applications.

### Compiling Tools

- [LiveReload](http://livereload.com/) - Preprocesses files as soon as it is saved and the browser is instantly updated without reloading the page.

###  Prototyping Tools
Expecting team recommendations, please [post your suggestions here](https://github.com/ProcessMAP/Design-Team/issues)


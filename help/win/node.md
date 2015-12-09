## 2. Node.Js - Low-level Server Platform
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

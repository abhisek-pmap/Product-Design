### 4. Node.Js - Low-level Server Platform
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

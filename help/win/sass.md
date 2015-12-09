### 6. Sass - Stylesheet Language

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

/*
Title: Workflows
Description: Time saving approaches for creating awesome stuff
*/


## Todo:

* Prototyping workflows for devices (web and apps)
	* Some paper and a pencil
	* Axure
	* OmniGraffle
	* inVision
* Responsive webdesign workflow (from design to deploy)
* Application planning and UML
* Deployment workflows using git, php and ...?


## Deploy Git over FTP

The best one I've found so far is based on NodeJS and called [DPLOY](http://leanmeanfightingmachine.github.io/dploy/) which is also available on [Github](https://github.com/LeanMeanFightingMachine/dploy). All settings are in YAML and it has support for multiple environments, perfect for local development with staging and production environments.

Note: if you install dploy in the same directory you want to sync, then leave path.local blank! [Read Github Issue](https://github.com/LeanMeanFightingMachine/dploy/issues/19#issuecomment-29133963).

You also have online services to deploy git project over FTP, but the most are quite expensive and not always so reliable:

- [dploy](http://dploy.io/)
- [FTPLOY](http://ftploy.com/)
- [Beanstalk](http://beanstalkapp.com/)


## Using Yeoman

Installation is quite simple when you have NPM and Git installed: npm install -g yo

This will install Grunt and Bower automaticly. You'll also need Ruby and Compass when your planning to use SASS (SCSS).

[Getting started wiki](https://github.com/yeoman/yeoman/wiki/Getting-Started)

[Building apps with the Yeoman workflow](http://dev.tutsplus.com/tutorials/building-apps-with-the-yeoman-workflow--net-33254)

Examples of use:

- yo webapp
- npm install -g generator-ember
- yo ember
- yo ember:model
- grunt test
- grunt serve
- grunt (--force)

Nice Yo Generators

- [Ember](https://github.com/yeoman/generator-ember)
- More will follow... Check out the [community generators](http://yeoman.io/community-generators.html)


## Using Grunt

### Articles

- [Grunt is not weird and hard on 24 Ways](http://24ways.org/2013/grunt-is-not-weird-and-hard/)
- [Setting up Pure and SASS with Grunt](http://kalenjohnson.com/customizing-roots-sass/)

### Tasks shortlist:

- Javascript (jslint)
- CSS (preprocessor, minimize)
- Image optimizing (imagemin)
- Watch (watch config, livepreview)


## Using Bower

- bower search ...
- bower install ... (--save)
- bower list
- bower update ...
- grunt bower - Injects your Bower dependencies into your ... configuration
- grunt bower-install - Injects your dependencies into your index.html file


## Terminal Tricks (For OS X)

### A little cheatsheet with commands:

* **ls -a**: lists all files, including hidden files (-a).
* **open .**: open directory in OS X Finder.


### .bash_profile

This file located at the /~ (your user folder) manages all bash/commandline settings for your account. Below some basics and tricks:

**For easy editing this bash profile file and also reloading it you can add these lines. Edit using 'editprofile' and 'reloadprofile' reloads the settings after editing.**

	alias editprofile="sudo nano ~/.bash_profile"
	alias reloadprofile=". ~/.bash_profile"


**Adding applications so you can use inkscape, bower or yo like below, without the filepath.**

	alias inkscape="/Applications/Inkscape.app/Contents/Resources/bin/inkscape"
	alias bower="/usr/local/lib/node_modules/bower/bin/bower"
	alias yo="/usr/local/lib/node_modules/yo/bin/yo"


**It's also possible to add paths/directories so everything within will be accessable without the full filepath.**

	export PATH="/usr/local/bin:$PATH"
	export PATH="/usr/local/php5/bin:$PATH"
	export PATH="/usr/local/mysql/bin:$PATH"
	export PATH="/Applications/Xcode.app/Contents/Developer/usr/libexec/git-core/:$PATH"
	export PATH="/Users/tim/Documents/Mobile/android-sdk-macosx/tools/:$PATH"
	export PATH="/Users/tim/Documents/Mobile/android-sdk-macosx/platform-tools/:$PATH"

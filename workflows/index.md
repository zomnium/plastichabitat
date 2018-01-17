/*
Title: Workflows
Description: Time saving approaches for creating awesome stuff
*/


## Todo:

* Prototyping workflows for devices (web and apps)
	* [Some paper and a pencil](https://www.google.com/search?q=pencil+and+paper&tbm=isch)
	* [Axure](http://axure.com/)
	* [OmniGraffle](http://www.omnigroup.com/omnigraffle/)
	* [inVision](http://www.invisionapp.com/)
	* [FramerJS](http://framerjs.com/)
	* [Origami](http://facebook.github.io/origami/) prototyping toolkit for Quartz Composer
	* [CSS Wireframes](https://github.com/agauniyal/wireframe)
* A/B Testing
	* [Study](https://github.com/dollarshaveclub/study)
* Responsive webdesign workflow (from design to deploy)
* Application planning and UML
* Deployment workflows using git, php and ...?
* Code formatting
	* [Prettier](https://prettier.io/)


## Design Sprints

- [Duco](http://duco.newhaircut.com/) Your practical guide to running successful Design Sprints


## Deploy Git over FTP

The best one I've found so far is based on NodeJS and called [DPLOY](http://lucasmotta.github.io/dploy/) which is also available on [Github](https://github.com/lucasmotta/dploy). All settings are in YAML and it has support for multiple environments, perfect for local development with staging and production environments.

Note: if you install dploy in the same directory you want to sync, then leave path.local blank! [Read Github Issue](https://github.com/lucasmotta/dploy/issues/19#issuecomment-29133963).

You also have online services to deploy git project over FTP, but the most are quite expensive and not always so reliable:

- [dploy](http://dploy.io/)
- [FTPLOY](http://ftploy.com/)
- [Beanstalk](http://beanstalkapp.com/)


## Deployment and development

### Open Source Projects

* [Docker](https://www.docker.com/)
* [Deployer](http://deployer.org/) (for PHP)
* [Magallanes](http://magephp.com/) (for PHP)
* [Puppet](https://puppetlabs.com/)
* [Rocketeer](http://rocketeer.autopergamene.eu/) (for PHP)
* [Vagrant](https://www.vagrantup.com/)
* [PHP The Right Way: Virtualization](http://www.phptherightway.com/#virtualization)

### Services

* [Chef](https://www.chef.io/)
* [Envoyer](https://envoyer.io/)
* [Forge](https://forge.laravel.com/)

### Resources

* [Getting Git Right](https://www.atlassian.com/git/)


## Using Yeoman

Installation is quite simple when you have NPM and Git installed: `npm install -g yo`

This will install Grunt and Bower automaticly. You'll also need Ruby and Compass when your planning to use SASS (SCSS).

- [Getting started wiki](https://github.com/yeoman/yeoman/wiki/Getting-Started)
- [Building apps with the Yeoman workflow](http://dev.tutsplus.com/tutorials/building-apps-with-the-yeoman-workflow--net-33254)
- [Yeoman Ember -- The missing tutorial](https://www.openshift.com/blogs/day-24-yeoman-ember-the-missing-tutorial)

Examples of use:

- `yo webapp`
- `npm install -g generator-ember`
- `yo ember`
- `yo ember:model`
- `grunt test`
- `grunt serve`
- `grunt (--force)`

Nice Yo Generators

- [Ember](https://github.com/yeoman/generator-ember)
- [Html 5 Boilerplate](https://github.com/h5bp/generator-h5bp)
- [Sass Boilerplate](https://github.com/srsgores/generator-sass-boilerplate)
- [Underscores for WordPress](https://github.com/kdo/generator-wp-underscores)
- More will follow... Check out the [community generators](http://yeoman.io/community-generators.html)


## Taskmanagers

- [Choose: Grunt, Gulp, or npm?](http://ponyfoo.com/articles/choose-grunt-gulp-or-npm)
- [Broccoli](https://github.com/broccolijs/broccoli)
- [FuseBox](https://fuse-box.org/)
- [Gulp](https://gulpjs.com/)
- [Grunt](https://gruntjs.com/)
- [npm](https://docs.npmjs.com/misc/scripts)
- [Parcel](https://parceljs.org/)
- [Webpack](https://webpack.js.org/)


### Grunt

#### Articles

- [Grunt is not weird and hard on 24 Ways](http://24ways.org/2013/grunt-is-not-weird-and-hard/)
- [Setting up Pure and SASS with Grunt](http://kalenjohnson.com/customizing-roots-sass/)

#### Tasks shortlist:

- Javascript (jslint)
- CSS (preprocessor, minimize)
- Image optimizing (imagemin)
- Watch (watch config, livepreview)


### Gulp

[Building with Gulp](http://www.smashingmagazine.com/2014/06/11/building-with-gulp/)


## Terminal Tricks (For OS X)

### Useful tools

* [iTerm](http://iterm2.com/)
* [Oh my zsh](https://github.com/robbyrussell/oh-my-zsh)
* [ZSH-LOVERS](https://grml.org/zsh/zsh-lovers.html)

### A little cheatsheet with commands:

* `ls -a` - lists all files, including hidden files (-a).
* `open .` - open directory in OS X Finder.
* `cp` - copy a file or directory.
* `mv` - move a file or directory.


## Using Bower

- `bower search ...`
- `bower install ...` (`--save`)
- `bower list`
- `bower update ...`
- `grunt bower` - Injects your Bower dependencies into your ... configuration
- `grunt bower-install` - Injects your dependencies into your index.html file


### .bash_profile

This file located at the /~ (your user folder) manages all bash/commandline settings for your account. Below some basics and tricks:

**For easy editing this bash profile file and also reloading it you can add these lines. Edit using '`editprofile`' and '`reloadprofile`' reloads the settings after editing.**

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

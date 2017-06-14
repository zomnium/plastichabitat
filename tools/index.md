/*
Title: Tools
Description: Useful tools for creating and managing front-end and backend stuff
*/


## [Color Oracle](http://www.colororacle.org/)

 Color Oracle is a free color blindness simulator for Window, Mac and Linux. It takes the guesswork out of designing for color blindness by showing you in real time what people with common color vision impairments will see.
 

## [Composer](http://getcomposer.org)

The package and dependency-manager for PHP. More information and documentation can be found on [getcomposer.org](http://getcomposer.org) and packages can be browsed and added at [Packagist](https://packagist.org/).


## [FontPrep](http://fontprep.com/)

Open-source tool for OS X drag & drop webfont creation, with support for OTF and TTF files.


## [Git](http://git-scm.com/)

Version Control System, VCS in short, Git is used for controlling versions and different branches of development. This way you can manage your versions and can go back in time, also work on your project easily with multiple developers without conflicts.

Git is widely supported in the development world. If you need a Git server/cloud service check out [GitHub](http://github.com/), commonly used for open source projects. [BitBucket](http://bitbucket.com/) is also a cloud service, but has free unlimited private respositories. Of course it's also possible to run your own server (see GitLab below).

A nice way to work with git is the [Git Flow](http://nvie.com/posts/a-successful-git-branching-model/) approach. Which is also integrated in [SourceTree](http://www.sourcetreeapp.com/), a Git GUI for OS X. Want to practice your git commandline skills? [Github](https://github.com/) and [CodeSchool](https://www.codeschool.com/) made a nice webapp to do this: [Try Git in 15 Minutes](http://try.github.io/levels/1/challenges/1). Want to know more? Read this: [git - the simple guide](http://rogerdudler.github.io/git-guide/). When you've got the basics, read [Git Best Practices](http://sethrobertson.github.io/GitBestPractices/).

For creating a secure connection you'll need to generate a SSH key, GitHub has a nice article about it: [Generating SSH Keys](https://help.github.com/articles/generating-ssh-keys#platform-mac)


## [GitLab](https://www.gitlab.com/)

A self hosted version of GitHub, commercial and community licences are available. To get started read [How to Setup GitLab](http://scotch.io/tutorials/how-to-setup-gitlab-a-self-hosted-github) on Scotch.


## [Kap](https://getkap.co/)

An open-source screen recorder built with web technology.


## MAMP - Local development

Combine Mac OS X with Apache, MySQL and PHP and you'll have MAMP. There is an application with all-in-one, called [MAMP](http://www.mamp.info/en/index.html). Bitnami has [some stacks](https://bitnami.com/stacks/infrastructure) available too. I prefer to install and manage it myself using these:

* [PHP for OS X by Liip](https://github.com/liip/php-osx)
* [MySQL Community Edition](http://dev.mysql.com/downloads/mysql/)
* Pre-installed Apache with vhosts and /etc/hosts
* [Get MAMP working on Yosemite](http://coolestguidesontheplanet.com/get-apache-mysql-php-phpmyadmin-working-osx-10-10-yosemite/)


## [Matterwiki](http://matterwiki.com/)

A simple and beautiful wiki for teams. People use it to store documentation, notes, culture guidelines, employee onboarding content and everything they want to. Build upon React.js with Node.js and Sqlite3 as back-end.


## [npm](https://npmjs.org/)/[node](http://nodejs.org/)

Node is a fast and light-weight JavaScript application platform. Build on Google's V8 JavaScript engine, used in Chrome/Chromium. The package and dependency-manager for node is npm.

### Update npm/node

You can update npm like this:

	npm install npm -g

When you have problems with lockfiles afterwards. You can solve this by resetting the file owner ([see topic on stackoverflow](http://stackoverflow.com/questions/22152162/npm-cannot-install-dependencies-attempt-to-unlock-something-which-hasnt-been)). Which you can do like this:

	sudo chown -R `whoami\` ~/.npm

For node you'll have to do a little bit more:

	sudo npm cache clean -f
	sudo npm install -g n
	sudo n stable


## [Piwik](http://piwik.org/)

Open-source web analytics tool, online and app for mobile! Try it out, it even has an auto-updater.


## [Sketch](http://bohemiancoding.com/sketch/)

Vector based application for designing digital media, with all kinds nice features. Including an easy assets export. The software is available on the App Store for $79, a trial version is available on their website.

Also try [Sketch Toolbox](http://sketchtoolbox.com/), which is a super simple plugin manager for Sketch. With [Runner](http://sketchrunner.com/) you can speed up your workflow, read more about it on [medium](https://medium.com/sketch-app-sources/runner-speed-up-your-sketch-workflow-fba470ed43c1#.v9tddmwxb). [Introducing Auto-layout for Sketch](https://medium.com/sketch-app-sources/introducing-auto-layout-for-sketch-24e7b5d068f9) shows you how the [Auto-layout](https://animaapp.github.io/Auto-Layout/) plugin makes it easy to resize layouts.

* The plugin [User Flows](https://abynim.github.io/UserFlows/) helps you with generating flow diagrams from Artboards.
* [UX Flow](http://uxflow.co/) a flowchart kit for Sketch.
* [Lists](http://lists.design/), gallery of real data ready to be placed in your design.
* [Mirr.io](https://mirr.io/) turns Sketch designs into working prototypes, fast.
* [Mockuuups Studio](https://mockuuups.studio/sketch) turns Sketch artboards unto perspective mockups, real-time.
* [Slinky](https://finchalyzer.github.io/slinky/) export your Sketch designs  as HTML email templates.
* [React Sketch.app](http://airbnb.io/react-sketchapp/), render React components to Sketch; tailor-made for design systems.
* [Stark](http://getstark.co/) is a color-blind simulator and contrast checker for Sketch. Design with accessibility in mind.


## [Sublime Text](http://www.sublimetext.com/) *and code editors in general*

A lightning fast extendable and customizable text-editor. Nice alternatives are [Atom.io](https://atom.io/) which looks alot like Sublime Text, but is open-source and has a CLI and Git intergration (also check out [Seti UI](https://atom.io/themes/seti-ui)). Adobe funded [Brackets](http://brackets.io/) which is also open-source and is completely build in JavaScript. Commonly used paid editors are [Coda](https://panic.com/coda/) and [BBEdit](http://www.barebones.com/products/bbedit/).

### Plugins:

* [Emmet](http://emmet.io/) - also in combination with [Re:View](http://re-view.emmet.io/)
* [More useful Sublime Text plugins](http://net.tutsplus.com/tutorials/tools-and-tips/essential-sublime-text-2-plugins-and-extensions/)
* [Best of Sublime Text features, plugins and settings](https://scotch.io/bar-talk/best-of-sublime-text-3-features-plugins-and-settings) *on Scotch*
* [Working with Code Snippets in Sublime Text](http://www.hongkiat.com/blog/sublime-code-snippets/)

### Themes:

* [Ayu](https://github.com/dempfi/ayu)
* [Flatland Theme](https://github.com/thinkpixellab/flatland)
* [Material Theme](http://equinsuocha.io/material-theme/)
* [Predawn](http://jamiewilson.io/predawn/)
* [Spacegray Theme](http://kkga.github.io/spacegray/)
* [Solarized Theme](https://github.com/paulcpederson/solarized-sublime)
* [Best themes of 2015 and 2016](https://scotch.io/bar-talk/best-sublime-text-3-themes-of-2015-and-2016) *on Scotch*

### Hotkeys:

* Switching files: CMD+P
* Commands: CMD+SHIFT+P
* Switching projects: CMD+CTRL+P
* Find and multi-edit: CMD+F and after entering the keyword(s) use ALT+RETURN
* [More Sublime Text shortcuts](http://scotch.io/bar-talk/sublime-text-keyboard-shortcuts)

### My settings:

	{
		"bold_folder_labels": true,
		"color_scheme": "Packages/Theme - Flatland/Flatland Monokai.tmTheme",
		"flatland_square_tabs": true,
		"folder_exclude_patterns":
		[
			".sass-cache",
			"wp-admin",
			"wp-includes"
		],
		"font_size": 12.0,
		"ignored_packages":
		[
			"Vintage"
		],
		"scroll_past_end": true,
		"theme": "Flatland Dark.sublime-theme"
	}


## [SQLPad](http://rickbergfalk.github.io/sqlpad/)

SQLPad is a self-hosted web app for writing and running SQL queries and visualizing the results. Its goal is to be a simple tool for exploratory data work and visualizations, ideal for data analysts who would prefer to work in SQL.

SQLPad is meant to be run on an internal network for a single team. All connections added to the app can be used by all individuals with access to the SQLPad server. All queries written can be run and edited by everyone on the server. 


## [Typographic Supply](http://typography.supply/)

A great inventory of typographic tools, from font identifiers, online calculation and grid tools, javascript and css libraries to making typfaces.


## [Yarn](https://yarnpkg.com/)

A dependency manager for javascript. It is compatible with the npm package manager, and also can install bower packages. Although a slight different featuresset including lockfiles, checksums, flat mode and offline caching.


## Favicons

* [Favicon.cc](http://favicon.cc/)
* [Real Favicon Generator](http://realfavicongenerator.net/)


## Front-end Tools

* [Bower](http://bower.io/) - Web Package Manager / [What’s So Great About Bower?](http://css-tricks.com/whats-great-bower/)
* [Compass](http://compass-style.org/) - SASS Compiler
* [Grunt](http://gruntjs.com/) - JavaScript Task Runner
* [YEO](http://yeoman.io/) - Workflows with Yo, generate projects with Grunt and Bower


## Browser plugins

* [CSS Peeper](https://csspeeper.com/)
* [FontFaceNinja](http://fontface.ninja/)


## Online Tools

* [ASCII Emoticon Generator](https://ascii.li/emoticon-creator)
* [Amp What?](http://www.amp-what.com/)
* [Archetype](http://www.archetypeapp.com/)
* [Brandcolors](http://brandcolors.net/)
* [Ceasar CSS Animation](http://matthewlein.com/ceaser/)
* [CloudConvert](https://cloudconvert.com/)
* [Compressor.io](http://compressor.io/compress)
* [Cubic Bezier](http://cubic-bezier.com/)
* [Flexplorer](http://bennettfeely.com/flexplorer/)
* [Google Maps Builder](http://googlemapbuilder.mynameisdonald.com/)
* [Gridlover](http://www.gridlover.net/)
* [WP Hasty](https://www.wp-hasty.com/)
* [HTML 5 Outliner](http://gsnedders.html5.org/outliner/)
* [Icomoon](https://icomoon.io/)
* [Lorem Ipsum Generator](https://loremipsumgenerator.com/)
* [Material Palette](http://www.materialpalette.com/)
* [Nibbler](http://nibbler.silktide.com/)
* [Nucleo](https://nucleoapp.com/)
* [Page Weight](https://pageweight.imgix.com/)
* [Placeholdit](http://placehold.it/)
* [Programmer Excuses](www.programmerexcuses.com)
* [SVG 2 VectorDrawable](http://inloop.github.io/svg2android/)
* [xip.io](http://xip.io/) *wildcard dns for everyone*


## HTML5 Animation Tools

* [Google Web Designer](http://www.google.nl/webdesigner/) - Create HTML5 animations in a Flash kinda interface
* [Adobe Edge](http://html.adobe.com/edge/) - Create HTML5 animations in a Flash kinda interface
* [Keyshape](https://www.pixofield.com/) - Create animations for the Web


## Graphic Applications (open-source)

* [Inkscape](http://www.inkscape.org/) - Vector editor
* [FontForge](http://fontforge.org/) - Font editor
* [Gimp](http://www.gimp.org/) - Raster image editor


## Misc.

* [Captain](https://getcaptain.co/) - Manage Docker containers, instantly from the menu bar.
* [Macify](https://macify.io/) - rom web to macOS, onvert webapps to native macOS apps with ease.
* [Tad](http://tadviewer.com/) - A better way to view & analyze data.
* [tlapse](https://github.com/typicode/tlapse) - create a timelapse of your web development.


## I also like to use...

* [Dropbox](http://dropbox.com/)
* [Evernote](http://evernote.com/)
* [Gimmebar](https://gimmebar.com/)
* [Pocket](http://getpocket.com/)
* [Trello](http://trello.com/)
* [Wunderlist](http://wunderlist.com/)

/*
Title: Javascript
Description: Client side javascript and frameworks
*/


## Articles

### OOP

* [Introduction to Object-Oriented JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Introduction_to_Object-Oriented_JavaScript) *on MDN*
* [JavaScript Garden](http://bonsaiden.github.io/JavaScript-Garden/)
* [The Module Pattern](http://css-tricks.com/how-do-you-structure-javascript-the-module-pattern-edition/) *on CSS-Tricks*
* [Javascript module instances/objects](http://www.sefol.com/?p=1090)
* [Why I don't love JavaScript's Module Pattern](http://snook.ca/archives/javascript/no-love-for-module-pattern)
* [Javascript's this](http://www.2ality.com/2014/05/this.html)

### Misc.

* [Managing events in JavaScript](http://krasimirtsonev.com/blog/article/Managing-events-in-JavaScript-using-)


## Awesome stuff

* [Socket.io](http://socket.io/)
* [D3JS](http://d3js.org/)
* [Raphael](http://raphaeljs.com/)
* [localForage](http://mozilla.github.io/localForage/)
* [PlayerJS](http://playerjs.io/)
* [Watch.js](https://github.com/melanke/Watch.JS)
* [Metrics Graphics JS](http://metricsgraphicsjs.org/)


## Useful libraries and plugins

### Filter and sort

* [Isotope](http://isotope.metafizzy.co/)
* [Masonry](http://masonry.desandro.com/)
* [MixItUp](http://mixitup.io/)
* [Shuffle](http://vestride.github.io/Shuffle/)

### Editors

* [Ace](http://ace.c9.io/)
* [Code Mirror](http://codemirror.net/)
* [Medium.js](https://github.com/jakiestfu/Medium.js/)
* [Scribe](https://github.com/guardian/scribe)
* [ZenPen](http://www.zenpen.io/)

### Tools

* [Heatmap.js](http://www.patrick-wied.at/static/heatmapjs/)
* [Typeset.js](https://blot.im/typeset/)

### Touch and gestures

* [Hammer](http://eightmedia.github.io/hammer.js/)
* [Interact.js](http://interactjs.io/)
* [Slip](https://github.com/pornel/slip)
* [Sortable](http://rubaxa.github.io/Sortable/)

### User interface

* [SmoothState](http://weblinc.github.io/jquery.smoothState.js/index.html) page transitions ([introduction article on CSS-Tricks](http://css-tricks.com/add-page-transitions-css-smoothstate-js/))
* [Stretchy](http://leaverou.github.io/stretchy/) - Form element autosizing, the way it should be.
* [Tooltipser](http://iamceege.github.io/tooltipster/)

### Misc.

* [Agile](http://a-jie.github.io/Agile/) CSS3 Engine
* [Google Charts](https://developers.google.com/chart/interactive/docs/index)
* [Prerender](https://prerender.io/)
* [Breeze](http://www.breezejs.com/)
* [Slick](http://kenwheeler.github.io/slick/)
* [Webpack](http://webpack.github.io/)


## Frameworks

* [Ampersand](http://ampersandjs.com/)
* [Angular](http://angularjs.org/)
* [Backbone](http://backbonejs.org/)
* [Ember](http://emberjs.com/)
* [Rivets.JS](http://www.rivetsjs.com/)
* [Stapes.js](http://hay.github.io/stapes/)
* [React.js](http://www.ractivejs.org/)
* [Synapse](http://bruth.github.io/synapse/docs/)
* [Mean](http://mean.io/)
* [Vue](http://vuejs.org/) *(is a framework alike library)*

Check out [TodoMVC](http://todomvc.com/) for real examples!


### Good reads about MVC Frameworks

* [Ember vs. Angular](http://eviltrout.com/2013/06/15/ember-vs-angular.html)
* [Ember introduction](http://dev.tutsplus.com/tutorials/getting-into-ember-part-4--net-31517)
* [Learn Angular](http://www.learn-angular.org/)


### MVC - Angular

* [The ginormous and unstoppable list of useful Angular resources](http://www.planningforaliens.com/angular/ginormous-unstoppable-angular-resource-list/) *on Planning for Aliens*


### MVC - Ember

* [EmberWatch](http://emberwatch.com/)
* [Getting Into EmberJS](http://net.tutsplus.com/tutorials/javascript-ajax/getting-into-ember-js/) on Tutsplus


## HTML5 Spotlight

* [Object.observe](http://wiki.ecmascript.org/doku.php?id=harmony:observe)
* [Promises](http://www.html5rocks.com/en/tutorials/es6/promises/)
* [Native Drag & Drop](http://www.html5rocks.com/en/tutorials/dnd/basics/)
* [element.animate(), HTML Imports, and Object.observe()](http://blog.chromium.org/2014/05/chrome-36-beta-elementanimate-html.html)
* [Presentation API Tutorial](http://html5hub.com/presentation-api-tutorial/)


## Node

* [Express](http://expressjs.com/) application framework
* [Ghost](https://ghost.org/) publishing platform
* [Hexo](http://hexo.io/) bloging framework
* [ROOTS](http://roots.cx/) toolbox
* [Sails](http://sailsjs.org/) realtime framework
* [Wintersmith](http://wintersmith.io/) static site generator

### Update Node.js

The easiest way to update node through npm (by [David Walsh](http://davidwalsh.name/upgrade-nodejs)):

	sudo npm cache clean -f
	sudo npm install -g n
	sudo n stable


## D3 

* [Ember and D3](http://embervis.affin.io/) - [slides](http://embervis.affin.io/slides/#/)


## JS Fun

* [In browser DVD's](http://gmarty.github.io/jsconf-2014-talk-play-dvd-in-js/)
* [Screeps](http://screeps.com/) JavaScript game!


## Wrapper

	(function (window, document) {

		'use strict';

		// Code here please :)

	}(this, this.document));


## Module

	var module = function() {

		'use strict';

		var variable = 'hello';

		function hello(what) {
			return variable + ' ' + what;
		}

		return {
			say: hello
		}
	};

	var hello = new module();
	console.log(hello.say('world'));

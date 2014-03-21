/*
Title: Blueprints
Description: Components and snippets, responsive and for daily use
*/


## Todo: Make a reference with reusable (and responsive) snippets

* Grids
* Content sliders / Slideshows
* Lightboxes
* Modals
* Cookie notifications
* Icons (retina: svg/png)
* Fonts
* Fullscreen backgrounds
* Headline backgrounds
* Email protection
* Sharing and socials


## Easiest fallback for Internet Explorer (IE6 to IE8)

It takes a lot of time building for old IE browsers and debugging is a pain. Hacks and fallbacks will quickly take over your code. But if you design and build website with a content/mobile first approach there is an easy way out! Media queries are supported by IE9 and up, so that CSS won't be executed. In combination with Paul Irish's [IE conditional classes](http://paulirish.com/2008/conditional-stylesheets-vs-css-hacks-answer-neither/) and a few rules of CSS you can serve just simple mobile layouts:

	body {
		width: auto;
	}

	.lt-ie9 {
		background-color: #eeeeee;
	}

	.lt-ie9 body {
		background-color: #ffffff;
		margin: 0 auto;
		width: 450px;
	}

More information about this approach: [Leaving old IE behind](http://www.jonikorpi.com/leaving-old-IE-behind/) *by Joni Korpi*

You can also add a little browse happy notification for those people who are affected by this, if you use [Html5 Boilerplate](http://html5boilerplate.com/) you'll already have this piece of code. Put it right after the opening body tag. This way your visitors know they're not browsing the most beautiful version of your website.

	<!--[if lt IE 10]>
	<p class="browsehappy">You are using an <strong>outdated</strong> browser. Please <a href="http://browsehappy.com/">upgrade your browser</a> to improve your experience.</p>
	<![endif]-->

Add a little bit of styling and your done!

	.browsehappy {
	    background: #eee;
	    color: #333;
	    line-height: 1.5em;
	    margin: 0;
	    padding: 1em;
	    text-align: center;
	}

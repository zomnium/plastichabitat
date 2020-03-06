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


## Resources

* [CSS tooltip](http://codepen.io/mildrenben/pen/rVBrpK)
* [Inclusive components](https://inclusive-components.design/) - A blog trying to be a pattern library. All about designing inclusive web interfaces, piece by piece.


## Easiest fallback for Internet Explorer (IE6 to IE8)

It takes a lot of time building for old IE browsers and debugging is a pain. Hacks and fallbacks will quickly take over your code. But if you design and build website with a content/mobile first approach there is an easy way out! Media queries are supported by IE9 and up. So all that CSS code in the media queries won't be executed. In combination with Paul Irish's [IE conditional classes](http://paulirish.com/2008/conditional-stylesheets-vs-css-hacks-answer-neither/) and a few rules of CSS you can serve the mobile layout:

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

You can also add a little browse happy notification for those people who are affected by this, if you use [Html5 Boilerplate](http://html5boilerplate.com/) you'll already have this piece of code. Although Html5 Boilerplate uses lower then IE 10 by default. Put it right after the opening body tag. This way your visitors know they're not getting the full desktop experience.

	<!--[if lt IE 9]>
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

### Important note!

Recently I read some issues on GitHub from the HTML5 boilerplate project. Where they removed conditional classes:

* [Conditional comments wrapping <html> prevent IE from honouring <meta http-equiv=X-UA-Compatible>](https://github.com/h5bp/html5-boilerplate/issues/1187)
* [Remove IE conditional classes](https://github.com/h5bp/html5-boilerplate/issues/1290)

So I'm looking for better fallback technics (if it's needed at all). Some things that can come in handy:

* [Modernizr](http://modernizr.com/)
* [CSS Browser Selector](https://github.com/ridjohansen/css_browser_selector)

*To be continued!*


## Maintenance page, using .htaccess

When you're doing some maintenance on your website, it's nice to have all traffic redirected to a message that it will be back asap. This way they can't interupt anything and know about the current state (or else they will think the website is broken).

When using an Apache stack, the easiest way is to use `.htaccess`. See the example below, with this piece of configuration all requests will be redirected to `maintenance.html` (which will be the only accessible file).

	Options +FollowSymlinks
	RewriteEngine On
	RewriteBase /
	RewriteCond %{REQUEST_URI} !/maintenance.html$
	RewriteRule .* /maintenance.html [R=307,L]

So when you create a be right back message, just name it `maintenance.html` and make sure all needed css, javascript and assets are in there! All other files won't be accessible with this configuration.

### Don't lock yourself out

The only problem with the previous `.htaccess` configuration is that it will redirect everyone, including you. If you want to lock everybody out, except yourself. Then the following snippet could be useful:

	Options +FollowSymlinks
	RewriteEngine On
	RewriteBase /
	RewriteCond %{REMOTE_ADDR} !^11\.111\.111\.111
	RewriteCond %{REQUEST_URI} !^/maintenance\.html$
	RewriteRule .* /maintenance.html [R=307,L]

*Don't forget to replace the IP-address with your own*

### Maintenance page for WordPress

When you want to apply the tricks seen above to a WordPress website, you will get this:

	# Mod rewrite
	Options +FollowSymlinks
	RewriteEngine On
	RewriteBase /

	# Maintenance
	RewriteCond %{REMOTE_ADDR} !^11\.111\.111\.111
	RewriteCond %{REQUEST_URI} !^/maintenance\.html$
	RewriteRule .* /maintenance.html [R=307,L]

	# WordPress
	RewriteRule ^index\.php$ - [L]
	RewriteRule ^wp-admin$ wp-admin/ [R=301,L]
	RewriteCond %{REQUEST_FILENAME} -f [OR]
	RewriteCond %{REQUEST_FILENAME} -d
	RewriteRule ^ - [L]
	RewriteRule ^(wp-(content|admin|includes).*) $1 [L]
	RewriteRule ^(.*\.php)$ $1 [L]
	RewriteRule . index.php [L]

*And again, don't forget to replace the IP-address with yours!*

When you wan't to go back online, just comment out the Maintenance section by putting `#` before each line. Save and upload, done! You're back online :)

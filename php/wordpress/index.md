/*
Title: WordPress
Description: Handy plugins, resources and snippets for WordPress.
*/


## Useful resources

- [Make Sense of WP Query Functions](http://wordpress.stackexchange.com/questions/1753/when-should-you-use-wp-query-vs-query-posts-vs-get-posts) *on StackExchange*
- [Action Reference](http://codex.wordpress.org/Plugin_API/Action_Reference) *on WP codex*
- [Filter Reference](http://codex.wordpress.org/Plugin_API/Filter_Reference) *on WP codex*
- [Capabilities](http://codex.wordpress.org/Function_Reference/current_user_can) *on WP codex (current_user_can)*
- [10 things every WP developer should know](http://www.smashingmagazine.com/2011/03/08/ten-things-every-wordpress-plugin-developer-should-know/) *on SmashingMagazine*


## Developing themes

It can be a lot of work to start from nothing, therefore it can be useful to start from a boilerplate:

- [Customizing the Roots Theme Pure CSS and Sass/Compass](http://kalenjohnson.com/customizing-roots-sass/)
- [Cutlass](http://cutlasswp.com/) for OO templates with Blade and Gulp
- [Roots](http://roots.io/) Modern WordPress Development, *using Composer, Boilerplate, Bootstrap and Grunt*
- [Timber](https://github.com/jarednova/timber) for OO templates with Twig
- [Underscores](http://underscores.me/) Start Theme


## Developing plugins

- [The WordPress Plugin Boilerplate](http://wppb.io/)


## Useful plugins

### Development

- [Advanced Custom Fields](http://www.advancedcustomfields.com/) for full control of your edit screens &amp; custom field data
	- [Extending ACF](http://www.smashingmagazine.com/2015/09/extending-advanced-custom-fields-with-your-own-controls/) *on Smashing Magazine*
- [Asynchronous Tasks](https://github.com/techcrunch/wp-async-task) *by TechCrunch*
- [Meta Box](http://www.deluxeblogtips.com/meta-box) creates an easy API for custom meta fields
- [Posts 2 Posts](http://scribu.net/wordpress/posts-to-posts/) makes post relationships easy
- [Redux Framework](https://wordpress.org/plugins/redux-framework/)
- [Regenerate thumbnails](http://www.viper007bond.com/wordpress-plugins/regenerate-thumbnails/) in batches
- [WordPress Importer](http://wordpress.org/plugins/wordpress-importer/) let's you import exported content

### Editing

- [Advanced Responsive Video Embedder](https://wordpress.org/plugins/advanced-responsive-video-embedder/)
- [Conductor](http://slocumthemes.com/wordpress-plugins/conductor/)

### Security and Logging

- [Blackbox](https://wordpress.org/plugins/blackbox-debug-bar/)
- [Security Audit Log](http://wordpress.org/plugins/wp-security-audit-log/)
- [Wordfence](http://wordpress.org/plugins/wordfence/)

### Content plugins

- [ACF](http://www.advancedcustomfields.com/) powerful fields for developers
- [Akismet](http://akismet.com/) check's for spam messages
- [Gigpress](http://gigpress.com/) for artists and tour calendars
- [WP User Avatar](http://wordpress.org/plugins/wp-user-avatar/) easy custom avatars
- [Yoast SEO](https://yoast.com/wordpress/plugins/seo/) for better search engine optimalization

### Widget plugins

- [Jetpack Widget Visibility](http://wordpress.org/plugins/jetpack-widget-visibility/) manage visibility per widget
- [Multisite Posts](https://wordpress.org/plugins/multisite-posts/) receives posts across sites
- [TinyMCE Widget](https://wordpress.org/plugins/black-studio-tinymce-widget/)

### Admin UI

- [Post types reorder](https://wordpress.org/plugins/post-types-order/) using a dragg and drop interface
- [White label CMS](http://www.videousermanuals.com/white-label-cms/) for a branded experience
- [Titan Framework](http://www.titanframework.net/) for creating WP options, [intro on tutsplus](http://code.tutsplus.com/articles/a-beginners-guide-to-titan-framework-creating-an-admin-panel-with-titan--cms-24358).

### Performance

- [WordPress Optimization/WordPress Performance](http://codex.wordpress.org/WordPress_Optimization/WordPress_Performance)
- [WordPress Optimization/Caching](http://codex.wordpress.org/WordPress_Optimization/Caching)
- [WordPress Performance Improvements That Can Go Wrong](http://www.smashingmagazine.com/2014/03/21/wordpress-performance-improvements-that-can-go-wrong/)
- [Theme Performance](http://themeshaper.com/2014/02/06/theme-performance/)
- [Transients API](http://codex.wordpress.org/Transients_API)
- [Asynchronous Javascript](https://wordpress.org/plugins/asynchronous-javascript/)
- [WP Performance Pack](http://wordpress.org/plugins/wp-performance-pack/)
- [WP Super Cache](https://wordpress.org/plugins/wp-super-cache/)
- [WP Fastest Cache](https://wordpress.org/plugins/wp-fastest-cache/)
- [W3 Total Cache](https://wordpress.org/plugins/w3-total-cache/)
- [Wordfence](http://wordpress.org/plugins/wordfence/)
- [5 of the Most Popular WordPress Caching Plugins](http://www.sitepoint.com/5-of-the-most-popular-wordpress-caching-plugins/) *on Sitepoint*

### MultiSite/Network related

- [Broadcast MU](http://wordpress.org/plugins/broadcast-mu/)
- [Proper Network Activiation](http://wordpress.org/plugins/proper-network-activation/)
- [ThreeWP Broadcast](http://wordpress.org/plugins/threewp-broadcast/)

Manage remote WordPress installations with [ManageWP Worker](http://wordpress.org/plugins/worker/).

### Forms

- [Contact Form 7](https://wordpress.org/plugins/contact-form-7/)
- [Contact Form DB](https://wordpress.org/plugins/contact-form-7-to-database-extension/)


## Multilingual websites

- [Codestyling Localization](http://www.code-styling.de/deutsch/entwicklungen/wordpress-plugin-codestyling-localization)
- [Multilingual Press](https://wordpress.org/plugins/multilingual-press/)
- [Polylang](http://polylang.wordpress.com/)
- [Zanto](http://zanto.org/)


## Snippets

### Get a post from another multisite

You can do this:

	switch_to_blog( $site_id );
	$post = get_post( $post_id );
	restore_current_blog();

But this function is also in WP core:

	function get_blog_post( $blog_id, $post_id ) {
	    switch_to_blog( $blog_id );
	    $post = get_post( $post_id );
	    restore_current_blog();

	    return $post;
	}

More background information:

- [How to get a post from another site in the network](http://make.marketpress.com/multilingualpress/2014/07/how-to-get-a-post-from-another-site-in-the-network/)
- [Switch to blog performance](http://wordpress.stackexchange.com/questions/106834/switch-to-blog-performance-considerations-alternatives)
- [Before you create a network](http://codex.wordpress.org/Before_You_Create_A_Network)
- [Share some data between two blogs](http://wordpress.org/support/topic/share-some-data-between-2-blogs-on-one-install)

### Misc.

- [Customize Login Page](https://premium.wpmudev.org/blog/customize-login-page/)


## Posts

- [Get posts](http://codex.wordpress.org/Template_Tags/get_posts)
- [WP_Query](http://codex.wordpress.org/Class_Reference/WP_Query)
- [Using WP_Query](http://www.smashingmagazine.com/2013/01/14/using-wp_query-wordpress/) *on Smashing Magazine*


## API

- [Theming with the REST API – Meet Picard](http://themeshaper.com/2015/05/07/theming-with-the-rest-api-meet-picard/)
- [WP API](https://github.com/WP-API/WP-API) *on GitHub*
- [WP API Docs](http://wp-api.org/)


remove_action('template_redirect', 'redirect_canonical');

wp-login.php can be used to (re-)set the URIs. Find this line:

require( dirname(__FILE__) . '/wp-load.php' );

and insert the following lines below:

//FIXME: do comment/remove these hack lines. (once the database is updated)
update_option('siteurl', 'http://your.domain.name/the/path' );
update_option('home', 'http://your.domain.name/the/path' );


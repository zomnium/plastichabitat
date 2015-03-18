/*
Title: PHP
Description: Notes for all kinds of cms's
*/


## Todo: Collect

- Content Management Systems
	- [AnchorCMS](http://anchorcms.com)
	- [Backdrop](https://backdropcms.org/)
	- [Bolt](https://bolt.cm/)
	- [Drupal](http://drupal.org/)
	- [Fork](http://www.fork-cms.com/)
	- [MODx](http://modx.com/)
	- [PageKit](http://pagekit.com/)
	- [Perch](http://grabaperch.com/) *($79 per site)*
	- [Silverstripe](http://silverstripe.com/)
	- [WordPress](http://wordpress.org/)
- Markdown & File based
	- [Cutenews](http://cutephp.com/)
	- [Dropplets](http://dropplets.com/)
	- [Kirby](http://getkirby.com/) *($39 per site)*
	- [Koken](http://koken.me/)
	- [Leeflets](https://leeflets.com/)
	- [Pico](http://pico.dev7studios.com/)
	- [Statamic](http://www.statamic.com/)
	- [Robodt](http://robodt.io/)
- Generators ([nice overview](https://www.staticgen.com/))
	- [Carew](http://carew.github.io/) 
	- [Easybook](http://easybook-project.org/)
	- [Sami](https://github.com/fabpot/sami) API documentation generator
	- [Sculpin](https://sculpin.io/)
- Frameworks
	- [CakePHP](http://cakephp.org/)
	- [CodeIgniter](http://ellislab.com/codeigniter)
	- [Laravel](http://laravel.com/)
	- [PPI](http://ppi.io/)
	- [Symfony](http://symfony.com/)
- Micro Frameworks
	- [Fat-free](http://fatfreeframework.com/)
	- [Slim](http://slimframework.com)
	- [Silex](http://silex.sensiolabs.org/)
- PHP Extension Frameworks
	- [Yaf](http://yafdev.com/)
	- [Phalcon](http://phalconphp.com/en/)


### Say no to these:

- Joomla
- Mambo
- Homebrew shizzles


### Drupal

Some theming related resources:

- [Basic](https://drupal.org/project/basic) Starter Theme
- [Getting started with SASS and Compass on Drupal](http://thejibe.com/blog/11/1/getting-started-basic-sass-and-compass-drupal)
- [Starter Themes](https://drupal.org/node/323993)
- [The Definitive Guide to Drupal 7](http://themery.com/dgd7)
- [Zen](https://drupal.org/project/zen) Starter Theme
- [Zen Documentation](https://drupal.org/node/193318)

Sortable content types:

- [Weight](https://drupal.org/project/weight) module for adding the weight type to fields
- [Comparison of node ordering modules](https://drupal.org/node/398508)


### Wordpress

- [Underscores](http://underscores.me/) Start Theme
- [Roots](http://roots.io/) Modern WordPress Development, *using Composer, Boilerplate, Bootstrap and Grunt*
- [Customizing the Roots Theme Pure CSS and Sass/Compass](http://kalenjohnson.com/customizing-roots-sass/)


### Next level shit!

- [PHP OOP5](http://www.php.net/manual/en/language.oop5.basic.php)
- [PHP Traits](http://de3.php.net/traits)
- [A Beginner’s Guide to Design Patterns](http://net.tutsplus.com/articles/general/a-beginners-guide-to-design-patterns/)
- [The Repository Design Pattern](http://dev.tutsplus.com/tutorials/the-repository-design-pattern--net-35804)
- [Dependency Injection in PHP](http://dev.tutsplus.com/tutorials/dependency-injection-in-php--net-28146)
- [Design Patterns with PHP – Adapters](http://juniorgrossi.com/2013/design-patterns-with-php-adapters/)
- [Symfony DI Dependency Injection](http://symfony.com/doc/current/components/dependency_injection/introduction.html)
- [Symfony Service containers](http://symfony.com/doc/current/book/service_container.html)
- [PHP References Explained](http://www.php.net/manual/en/language.references.php)
- [PHP Property Visibility](http://php.net/manual/en/language.oop5.visibility.php)
- [PHP Traits](http://php.net/manual/en/language.oop5.traits.php)
- More resources: [PHP The Right Way](http://www.phptherightway.com/)
- [HHVM](http://hhvm.com/)
- [Indatus](http://indatus.github.io/) (PHP Tools: Ranger, Blacksmith, Trucker, Foreman, Dispatcher)


## Realtime frameworks

- [Elephant](http://elephant.io/) - *Socket.io client*
- [PHP Deamon](http://daemon.io/)
- [ReactPHP](http://reactphp.org/)
- [Ratchet](http://socketo.me/)


## Configuration

### Change max upload file size

You'll have to edit your `php.ini` file, in three places:

- `upload_max_filesize` to set the maximum filesize
- `post_max_size` for handling the forms
- `memory_limit` is important to check too

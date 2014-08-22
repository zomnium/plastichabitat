/*
Title: PHP
Description: Notes for all kinds of cms's
*/


## Todo: Collect

- Content Management Systems
	- [AnchorCMS](http://anchorcms.com)
	- [Drupal](http://drupal.org/)
	- [MODx](http://modx.com/)
	- [Perch](http://grabaperch.com/) *($79 per site)*
	- [Silverstripe](http://silverstripe.com/)
	- [WordPress](http://wordpress.org/)
- Markdown & File based
	- [Cutenews](cutephp.com/)
	- [Dropplets](http://dropplets.com/)
	- [Kirby](http://getkirby.com/) *($39 per site)*
	- [Koken](http://koken.me/)
	- [Leeflets](https://leeflets.com/)
	- [Pico](http://pico.dev7studios.com/)
	- [Robodt](http://robodt.io/)
- Frameworks
	- [CakePHP](http://cakephp.org/)
	- [CodeIgniter](http://ellislab.com/codeigniter)
	- [Symfony](http://symfony.com/)
	- [Laravel](http://laravel.com/)
- Micro Frameworks
	- [Fat-free](http://fatfreeframework.com/)
	- [Slim](slimframework.com)
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
- More resources: [PHP The Right Way](http://www.phptherightway.com/)


## Configuration

### Change max upload file size

You'll have to edit your `php.ini` file, in three places:

- `upload_max_filesize` to set the maximum filesize
- `post_max_size` for handling the forms
- `memory_limit` is important to check too

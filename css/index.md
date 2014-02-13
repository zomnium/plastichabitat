/*
Title: CSS
Description: All about styling with CSS
Date: 2014-2-1
*/


## Todo: add more subjects

- Crossbrowser compatibility
- Fonts
- Icons
- Retina
- Forms
- Print
- Mobile first approach
- Content first, start here, work your way up



## Reset or Normalize

- [Eric Meyer's Reset](http://meyerweb.com/eric/tools/css/reset/)
- [Normalize](http://necolas.github.io/normalize.css/)
- [HTML5 Boilerplate](http://html5boilerplate.com/) can be useful to, it makes use of Normalize together with some other quickstart defaults.



## Box-sizing, use it!

Just use box-sizing, on everything. It's available in all new browsers and it's awesome! Block elements (like divs) will be way more predictable when you apply it to all elements and is recommed by Paul Irish and Chris Coyier. You know how hard it is to align forms? When you use this, it won't! Just do it already!

    *, *:before, *:after {
        -webkit-box-sizing: border-box; 
        -moz-box-sizing: border-box;
        box-sizing: border-box;
    }

More resources about the subject:

- [Box-sizing awareness day](http://css-tricks.com/international-box-sizing-awareness-day/) *on CSS-Tricks*
- [Box-sizing](http://css-tricks.com/box-sizing/) *on CSS-Tricks*
- [Box-sizing border-box ftw](http://www.paulirish.com/2012/box-sizing-border-box-ftw/) *by Paul Irish*
- [HTML5 Please](http://html5please.com/#box-sizing) *on HTML5 Please*
- [Box-sizing polyfill](https://github.com/Schepp/box-sizing-polyfill) *on GitHub*
- [Box-sizing border-box for IE8](http://stackoverflow.com/questions/11608291/box-sizing-border-box-for-ie8) *on StackOverflow*
- [Can I use](http://caniuse.com/#feat=css3-boxsizing)



## Using em for everything

- Using ems, use it for everything.
- Using ems for mediaqueries.

In pure CSS it can be a little time consuming, calculating everything. But with Sass it can be quite easy using this function:

    @function em($target, $context: 16) {
        @return ($target / $context) * 1em;
    }

    h1 {
        font-size:em(30);
    }

It's also possibly to use this approach inline like this:

    h1 {
        font-size:(30 / 14) * 1em;
    }

More information about [Calculating EMs with SCSS](http://erskinedesign.com/blog/calculating-ems-scss/).



## Vertical rhythm, the basics

Or baseline, is very important for the balance and readablity of a webpage. Below you can find a little example (which only works in combination with reset or normalize, of course):

    body {
        font-size: 100%; /* Use browsers default font-size, probably 16px */
        line-height: 1.5em; /* This will be 24px and is also our baseline! */
    }

    h1 {
        font-size: 3em;
        line-height: 1em;
        margin-bottom: 0.5em;
    }

    p {
        font-size: 1em;
        line-height: 1.5em;
        margin-bottom: 1.5em;
    }

Todo: add more notes and information.

Also check out [Modular Scale](http://modularscale.com/), which also has a Sass implementation: [Modular Scale Calculator](https://github.com/Team-Sass/modular-scale).



## Modulair CSS

Several approaches are available to write modulair CSS (it's a way of working, not a tool):

- [SMACCS](http://smacss.com/)
- BEM
    - [Getting your head ’round BEM syntax](http://csswizardry.com/2013/01/mindbemding-getting-your-head-round-bem-syntax/) *by CSS Wizardry*
    - [Our principles for BEM + Sass](http://blog.14islands.com/post/70395374262/our-principles-for-bem-sass) *by 14islands*
    - [Sassier (BE)Modifers](http://viget.com/extend/bem-sass-modifiers) *by Viget*
- OOCS
- Working method
- Part sheets



## Grids

### Using a framework

There's a lot of choice, below a little overview with well-known frameworks you can build upon:

- [960gs](http://960.gs/)
- [Bootstrap](http://getbootstrap.com/)
- [Fluid Baseline Grid](http://fluidbaselinegrid.com/)
- [Foundation](http://foundation.zurb.com/)
- [Golden Grid System](http://goldengridsystem.com/) *- Grid concept*
- [Goldilocks](http://goldilocksapproach.com/)
- [GuideGuide2](http://guideguide.me/) *- Grids extension for Photoshop*
- [Gumpy](http://gumbyframework.com/)
- [Pure](http://purecss.io/)
- [Skeleton](http://www.getskeleton.com/)
- [UIKit](http://www.getuikit.com/)


### Building your own grid

Some interesting approaches for settings up your custom grid:

- [Don't overthink grids](http://css-tricks.com/dont-overthink-it-grids/)
- [GRID - A simple guide to responsive design](http://www.adamkaplan.me/grid/)
- [Golden Grid System](http://goldengridsystem.com/)
- [Golden Grid System explained](http://seangoresht.com/index.php/tutorials/item/the-golden-gridlet-system-ggs-explained)

Some background information about grids and using types:

- [Fluid grids](http://alistapart.com/article/fluidgrids)
- [How to use text in CSS](http://alistapart.com/article/howtosizetextincss)
- [Sub-pixel problems in CSS](http://ejohn.org/blog/sub-pixel-problems-in-css/)
- [Setting type on the web](http://alistapart.com/article/settingtypeontheweb)



## Preprocessors

### [Sass](http://sass-lang.com/)

Todo: add some more information about Sass. For now, read this: [Sass Style Guide](http://css-tricks.com/sass-style-guide/) *on CSS-Tricks*.


### [AbsurdJS](http://krasimir.github.io/absurd/)

This preprocessor is quite different from the others. Most other preprocessors are written for CSS alike formats. AbsurdJS uses a JSON format, which is what makes it so powerful. You can use JavaScript! Besides styles in JSON and JavaScript functions support it also renders very very clean CSS. For big projects this can make a lot of difference.


### [LESS](http://www.lesscss.org/)

It's a very basic preprocessor, when you're a performance user you'll probably be better of with Sass. When you're not, probably too, Sass is awesome.



## Modernizr

Working with Modernizr can also be quite helpful when you need to support prehistoric browsers. With this tool you can detect functionalities/features, like SVG-support, media-queries or even box-sizing. When it doesn't, you can load a shiv (some javascript) to implement a fallback.

- [Modernizr](http://modernizr.com/)
- [Detect box-sizing](http://modernizr.com/download/#-shiv-mq-cssclasses-teststyles-testallprops-css_boxsizing-load)
- [Detect media-queries](http://stackoverflow.com/questions/7460670/how-to-detect-if-media-queries-are-present-using-modernizr)
- Todo: add a getting started tutorial/reference



## Misc.

- [Responsive Web-design](http://www.abookapart.com/products/responsive-web-design) *on A Book Apart*
- [Sass Boilerplate](https://github.com/srsgores/sass-boilerplate/) *on GitHub*

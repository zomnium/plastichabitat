/*
Title: HTML5
Description: All about HTML5
*/


## Todo: Make a reference about semantics etc.


## Web components

* [LitElement](https://lit-element.polymer-project.org/) - A simple base class for creating fast, lightweight web components
* [Polymer Project](https://www.polymer-project.org/) - Libraries, tools, and standards for a better web
* [Stencil](https://stenciljs.com/) - A toolchain for building reusable, scalable Design Systems.


## Outlining

Todo: write something about [outlining content](http://html5doctor.com/outlines/) and semantic structures. Nice tool: [HTML 5 Outliner](http://gsnedders.html5.org/outliner/)


## Doctype

	<!DOCTYPE html>


## Root element

	<html lang="en">

Check W3C's [Language Tags](http://www.w3.org/International/questions/qa-choosing-language-tags)


## Head elements

- Character Encoding / Meta charset
- Link relations
	- Stylesheet
	- Alternate
	- Rel: 
		- Author
		- Start
		- Prev
		- Next
	- Nofollow
	- Shortcut icon
	- Prefetch
	- Search


## Html5 Semantic Elements

### Section

Represents a thematic grouping of content, often with a heading. Could be chapters or tabbed interfaces. Webpages could be split into several sections like introduction, news items, latest posts, etc.

### Nav

This element is for a page section with links, to other pages or area's within the current document. Only major navigation blocks can use the nav element, paginations and footer links don't need it.

### Article

Represents a document, page, post, forumpost, article etc. and is intended to be indenpent or reusable. 

### Aside

Is a section of the page that contains content that can be related to the main content, but is considered separate.

### Hgroup - *don't use this*

**Important: this tag has been removed from the spec, do not use.** It would be used to group multiple levels of headlines, subheadings, alternative titles and taglines (h1 - h6).

### Header

Can be used for headers with logo's, navigation and search forms. But also for a sections heading.

### Footer

Typically contains information about the author, links to resources, coprights, etc. Can be used for sections and for documents.

### Time

Can be used with a 24 hour clock notation or Gregorian calendar, also has an optional time-zone attribute. Commonly used for publication dates etc.


## More semantic elements

### Main

Wraps the main page content and there can only be one in a document. It must not be a descendent of an `<article>`, `<aside>`, `<footer>`, `<header>` of `<nav>`. More the main element can be found on [Mozilla's MDN](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/main).

### Figure caption

...


## Media

- Video
- Audio

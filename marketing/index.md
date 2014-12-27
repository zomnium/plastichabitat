/*
Title: Marketing
Description: Best practices and useful information for online marketing
*/


## Analytics

It's always a good idea to measure your traffic. To see which pages are most important, where do your visitors come from and where do they leave? Also if your doing a campaign, send a newsletter or use other kinds of promotion it's good to see what works and what doesn't.

### Tools

The most populair tools for analyzing your website:

- Google Analytics
- Piwik
- GoSquared

### Things to find out

- Campaigns
- Conversion rate
- Sources
- Tracking (advanced)
- E-commerce


## Socials

All kinds of social media platforms popped up last years and became very important for marketing purposes. When you're creating websites and online promotions it's therefore important to optimize some things.

### OpenGraph

- Fields
- Images
- Best use
- CMS implementations (WordPress/Drupal)

### Facebook

- Use OpenGraph meta fields
- Optimize images for OpenGraph
- Profile picture sizes
- Obey the rules

### Twitter

- Use OpenGraph equivalent
- Optimize images for it
- Profile picture sizes


## Sharing

I like to keep it simple, just some anchors with classes. Easy to style and quick to load. It gets the job done, as it should. The only thing you'll have to do is replacing the values of `[message]`, `[permalink]`, `[username]` and `[title]`. Optionally you can personalize the classnames of course.

Good to know: Facebook uses OpenGraph (OG in short) for getting titles, images and other data. This way you'll get a nice featured spot on the timeline. So be sure to implement this!

	<p class="share-this">
		<span class="share-this-label">Share this on&hellip;</span>
		<a target="_blank" class="button button--social button--tweet" href="https://twitter.com/intent/tweet?text=[message]&url=[permalink]&via=[username]">Twitter</a>
		<a target="_blank" class="button button--social button--facebook" href="http://www.facebook.com/sharer/sharer.php?u=[permalink]">Facebook</a>
 		<a target="_blank" class="button button--social button--google" href="https://plus.google.com/share?url=[permalink]">Google+</a>
		<a target="_blank" class="button button--social button--linkedin" href="http://www.linkedin.com/shareArticle?mini=true&url=[permalink]&title=[title]&source=[permalink]">LinkedIn</a>
	</p>

---
layout: page
title: "Type Theme"
permalink: /project/type/
hide: true
---

![Default Type Theme blog](https://cloud.githubusercontent.com/assets/816965/5142407/19742e48-71d6-11e4-8d9d-fdfe010784f0.png)

A free and open-source [Jekyll](http://jekyllrb.com) theme. Great for blogs and easy to customize.

<a href="/type-theme/" class="button">Demo</a>
<a href="https://github.com/rohanchandra/type-theme" class="button">View on Github</a>

## New to Jekyll, Git or Github Pages?

If you are new to Jekyll and/or Git and would like to host your Jekyll blog using Github Pages, view a detailed installation walkthrough for Type Theme at:

<a href="/project/type/github/" class="button">Using Type Theme with Github Pages</a>

## Installing Type Theme

If you are familiar with Jekyll and Git, to use Type Theme with Jekyll:

1. [Install Jekyll](http://jekyllrb.com/docs/installation/), using `gem install jekyll`
2. Fork and clone the [Type Theme repo](https://github.com/rohanchandra/type-theme)
3. Customize the theme
4. Run the Jekyll server using `jekyll serve`
5. Visit [http://localhost:4000](http://localhost:4000) to view the site

## Customizing Type Theme

Open `_config.yml` in a text editor to change most of the blog's settings.

If a variable in this document is marked as "optional", disable the feature by removing all text from the variable. For example, to prevent the avatar from rendering in the header, the avatar line should read:

<pre>
theme:
  title: Type Theme
  avatar:  
  gravatar: 
</pre>

Notice the avatar variable is left intentionally blank. 

Below is a summary of the configuration options in Type Theme.

### Site configuration
The most common configurations, included here for guidance, are:

Jekyll website *without* a subpath (like this website):
<pre>
# SITE CONFIGURATION
baseurl: ""
url: "https://username.github.io"
</pre>

Jekyll website *with* subpath (like the Type Theme demo page):
<pre>
# SITE CONFIGURATION
baseurl: "/sub-directory"
url: "https://username.github.io/"
</pre>

Please configure this in `_config.yml` before using the theme.

### Meta

Meta variables hold basic information about your Jekyll site which will be used throughout the site and as meta properties for search engines, browsers, and the site's RSS feed.

Change these variables in `_config.yml`: 

Variable | Example | Description | Optional
-|-|-|
title | My Jekyll Blog | Name of website | Yes
avatar | avatar.png | Name of avatar image in the `/img` directory, to be displayed in the theme's header | Yes
gravatar | f9879d71855b5ff21e4963273a886bfc | [MD5 hash of your email address](https://secure.gravatar.com/site/implement/hash/) to load your Gravatar in the theme's header | Yes
description | My blog posts  | Short description, primarily used by search engines | Yes

### Header and footer text

Change these variables in `_config.yml`: 

Variable | Example | Description | Optional
-|-|-|
header_text | Welcome to my Jekyll blog | HTML (shown below the navigation) with a background colour for emphasis | Yes
footer_text | Copyright 2014 | HTML (shown at end of the site) with lighter text | Yes

### Icons

Add your username on selected websites in the icon section of the `_config.yml` file to display the site's icon from [Font Awesome](https://fortawesome.github.io/Font-Awesome/) in the header navigation. All icon variables should be your username enclosed in quotes (e.g. "username"), except for the following variables:

Variable | Example | Description | Optional
-|-|-|
rss | true | Takes boolean value (true/false) to show RSS feed icon | Yes
email_address | type@example.com | Email address |  Yes
linkedin | https://www.linkedin.com/in/FirstLast | Full URL to profile on LinkedIn | Yes
stack_exchange | https://stackoverflow.com/users/0000/first-last | Full URL to profile on Stack Exchange | Yes

### Scripts

Change these variables in `_config.yml`: 

Variable | Example | Description | Optional
-|-|-|
google_analytics | UA-123456-01 | Google Analytics [tracking ID](https://support.google.com/analytics/answer/1032385?hl=en) | Yes
disqus_shortname | shortname | Disqus [shortname](https://help.disqus.com/customer/portal/articles/466208-what-s-a-shortname-)|  Yes

Scripts listed here are only loaded if you provide a value in the `_config.yml` file.

### Localization strings

Change localization string variables in `_config.yml`.

English text used in the theme (such as the "continue reading" label) has been grouped  so you can quickly translate the theme or change labels to suit your needs.
  
### Colors, typography, padding

![A selection of colors set in Type Theme by modifying the CSS](https://cloud.githubusercontent.com/assets/816965/5142488/130869a6-71d7-11e4-8a38-a69ec1673436.png)

Navigate to the `_sass > base` directory and open `_variables.scss` to change colors, typography and padding used in the theme with CSS.

Mozilla's [ColorPicker](https://developer.mozilla.org/en-US/docs/Web/CSS/Tools/ColorPicker_Tool) is a helpful tool to get your preferred colours in hexadecimal or RGBA form for use in `_variables.scss`.

### Favicon

To change your favicon, usually displayed in the browser, place an ICO file named `favicon.ico` in the root directory of your blog.

## Posts and pages in Type Theme
[Jeykll docs for writing posts](http://jekyllrb.com/docs/posts/).

### Feature images

![Posts with geometric feature images](https://cloud.githubusercontent.com/assets/816965/5142406/19726478-71d6-11e4-8111-94f788b0e44d.png)

Add a feature image by specifying a path to an image in the [front matter](http://jekyllrb.com/docs/frontmatter/) in the form of `feature-img: "img/PATH_TO_IMAGE.png"`.

For example:

	---
	layout: post
	title: Hello World
	feature-img: "img/sample_feature_img.png"
	---


### Hiding pages from navigation

In the Front Matter of a page, add `hide: true` to prevent the page from showing up in the header's navigation bar (visitors can still visit the URL through other means).

For example:

    ---
    layout: page
    title: "Error 404: Page not found"
    permalink: /404.html
    hide: true
    ---
    
## License
[The MIT License (MIT)](https://github.com/rohanchandra/type-theme/blob/master/LICENSE)
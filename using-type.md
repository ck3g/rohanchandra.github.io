---
layout: page
title: "Type Theme"
permalink: /project/type.html
hide: true
---

![Default Type Theme blog](https://cloud.githubusercontent.com/assets/816965/5142407/19742e48-71d6-11e4-8d9d-fdfe010784f0.png)

Type Theme is a free and open-source [Jekyll](http://jekyllrb.com) theme, that's highly customizable and built for blogging.

[Demo](https://rohanchandra.github.io/type-theme/)


## Getting Started
1. [Install Jekyll](http://jekyllrb.com/docs/installation/), using `gem install jekyll`
2. Fork and clone the [Type Theme repo](https://github.com/rohanchandra/type-theme) **or** use the [Download ZIP](https://github.com/rohanchandra/type-theme/archive/master.zip) option on Github.com
3. Customize the theme
4. Run the Jekyll server using `jekyll serve`
5. Visit [http://localhost:4000](http://localhost:4000) to view the site

## Customizing Type Theme

### _config.yml
Open `_config.yml` in a text editor to change most of the blog's settings. Below is a summary of the configuration options.

**Meta**

Basic information about your Jekyll site which will be used throughout the site and as meta properties for search engines, browsers, and the site's RSS feed.

**Header and footer text** 

The header text is a large description, only shown at the top of the index page of your site, with a separate text and background color.

Both header and footer text support the use of HTML tags.

Removing all text either variable in the `_config.yml` file will hide the feature.

**Icons**

Add your username on selected websites in the icon section of the `_config.yml` file to display the site's icon from [Font Awesome](https://fortawesome.github.io/Font-Awesome/) in the header navigation.

In the `_config.yml` file, all social network usernames should be enclosed in quotes (e.g. "username"), except for LinkedIn and Stack Exchange which require a full URL.

The RSS variable takes a boolean value, i.e. `true` to display the icon or `false` to remove the icon.

**Scripts**

Scripts listed here are only loaded if you provide a value in the `_config.yml` file.

Google Analytics requires a [tracking ID](https://support.google.com/analytics/answer/1032385?hl=en), which is in the form of `UA-000000-01`.

A [Disqus shortname](https://help.disqus.com/customer/portal/articles/466208-what-s-a-shortname-) is required to enable the comments script. 

**Localization strings** 

English text used in the theme (such as the "continue reading" label) has been grouped  so you can quickly translate the theme or change labels to suit your needs.

### Colors, typography, padding

![A selection of colors set in Type Theme by modifying the CSS](https://cloud.githubusercontent.com/assets/816965/5142488/130869a6-71d7-11e4-8a38-a69ec1673436.png)

Navigate to the `_sass > base` directory and open `_variables.scss` to change colors, typography and padding used in the theme with CSS.

### Images
Change your avatar, which is shown in the theme's header, by adding the `avatar.png` file in the `/img` directory (if you're using a different file, specify the file name in `_config.yml`). Delete the file to remove the avatar from the header.

To change your favicon, usually displayed in the browser, place an ICO file named `favicon.ico` in the root directory of your blog.

## Writing with Type Theme
[Jeykll docs for writing posts](http://jekyllrb.com/docs/posts/).

**Feature images**

![Posts with geometric feature images](https://cloud.githubusercontent.com/assets/816965/5142406/19726478-71d6-11e4-8111-94f788b0e44d.png)

Add a feature image by specifying a path to an image in the [front matter](http://jekyllrb.com/docs/frontmatter/) in the form of `feature-img: "img/PATH_TO_IMAGE.png"`.

For example:

	---
	layout: post
	title: Hello World
	feature-img: "img/sample_feature_img.png"
	---


**Hide pages from navigation**

In the Front Matter of a page, add `hide: true` to prevent the page from showing up in the header's navigation bar (readers can still visit the URL through other means).

For example:

    ---
    layout: page
    title: "Error 404: Page not found"
    permalink: /404.html
    hide: true
    ---
    
## License
The MIT License (MIT)
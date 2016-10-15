# Strata Hexo Theme

Hexo implementation of the free [HTML5Up Strata Template](http://html5up.net/strata)

## Features Overview

- Disqus and Facebook comments
- Google Analytics
- Cover image for posts and pages
- Tags
- Categories
- Responsive Images
- Gravatar
- Social Media links
- Pagination

## Installation

### SCSS support

The `hexo-renderer-scss` is required.

Install it by using:

```
$ npm install --save hexo-renderer-scss
```
### Install the theme

Install the theme by using:

```
$ git clone https://github.com/livingos/hexo-theme-strata themes/strata
```

Then update your blog's main `_config.yml` to set the theme to `strata`:

i.e:

```
# Extensions
## Plugins: http://hexo.io/plugins/
## Themes: http://hexo.io/themes/
theme: strata
```

## Theme Configuration

The theme's global configuration is done in `/themes/hexo-theme-strata/_config.yml`.

### Gravatar email

Set the email address for your Gravatar configured in the theme's `_config.yml`.

```
# Gravatar email
gravatar_email: a@123.com
```

### Default index page cover image

You can specify a default thumbnail for posts on the index page (Home page). This image will be used if you forget to specify an image in the post's front matter.

```
# Default post cover index page
default_cover_index: "http://placehold.it/450x450"
```

### Default post page cover image

You can specify a default thumbnail for posts/pages on the post/page page (Detail Page). This image will be used if you forget to specify an image in the post's front matter. If you don't specify a default and you don't specify an image in your post, no image will be displayed

```
# Default post cover index page
default_cover_detail: "http://placehold.it/1300x500"
```

### Show Dates

By default, Strata does not show dates for posts and pages. You can set this config to true if you need to.

```
# Show Dates for posts and pages
show_dates:
```

### Comments

The comments provider is specified in the theme's `_config.yml`. If you specify both a `disqus_shortname` and a `facebook.appid` there will be 2 sets of comment per post. So choose one.

```
# Comments. Choose one by filling up the information
comments:
  # Disqus comments
  disqus_shortname: discussname
  # Facebook comments
  facebook:
    appid: 123456789012345
    comment_count: 5
    comment_colorscheme: light
```

### Google Analytics

The Google Analytics Tracking ID is configured in the theme's `_config.yml`.

```
# Google Analytics Tracking ID
google_analytics:
```

### Social Account

Setup the links to your social pages in the theme's `_config.yml`. Links are in the footer.

```
# Social Accounts
twitter_url:
facebook_url: https://www.facebook.com/
instagram_url:
dribble_url: https://dribbble.com/pixelhint
github_url:
googleplus_url: https://plus.google.com/+Pixelhint/posts
behance_url: https://www.behance.net/
fivehundredpx_url:
email_url:
rss_url:
```

## Post Custom Configuration

For each post, you can specify additional information in the [front matter](https://hexo.io/docs/front-matter.html)


### Post's Index Thumbnail

Use `cover_index` to specify an image that will be used for that post on the Home page (also knows as index)

Example:

```
cover_index: /assets/work1.jpg
```

### Post's Detail Thumbnail

Use `cover_detail` to specify an image that will be used for that post on the Detail page for that post.

```
cover_detail: /assets/hero_image.jpg
```

## Creator

This theme was created by [HTML5 Up](http://html5up.net/strata/) and adapted for Hexo by [Tim Hyde](http://livingos.com/).

Simple minimalistic dark theme for [Hugo](https://gohugo.io/).

![screenshot](https://github.com/bickhaus/hugo-dusk/blob/master/images/tn.png "screenshot")

## Features

* Responsive minimalistic design
* Configure theme colors via CSS file
* Syntax highlight with builtin [Chroma](http://gohugo.io/content-management/syntax-highlighting/)
* [OpenGraph](http://ogp.me/), [Twitter cards](https://dev.twitter.com/cards/overview) support
* [Disqus](https://disqus.com/) comments support
* [Google analytics](https://www.google.com/analytics/) (async)
* Configurable pagination for posts
* Lazy menu
* Custom 404 page
* Font Awesome icons in top social header

## Installation

~~~sh
$ mkdir themes
$ cd themes
$ git clone https://github.com/bickhaus/hugo-dusk.git
~~~

## Configuration

Example configuration:

~~~~toml
baseurl = "/"
title = "My site."
copyright = "Copyright (c) 2018. See <a href=#>someSite</a> for more information."
canonifyurls = true
languageCode = "en-US"
paginate = 3
theme = "hugo-dusk"
enableRobotsTXT = true

googleAnalytics = ""
disqusShortname = ""

[author]
  name = ""

SectionPagesMenu = "main"

# use Chroma for syntax highlight
pygmentsStyle = "native" # other dark style options: vim, fruity, monokai
# enable syntax highlight for code blocks
pygmentsCodeFences = true

[[menu.main]]
  name = "Posts"
  weight = -120
  identifier = "post"
  url = "/post/"

[[menu.main]]
  name = "Tags"
  weight = -110
  identifier = "tag"
  url = "/tags/"

[params.meta]
  keywords = "blog, tech"
  description = "Personal blog."

[params]
  github = "github id"
  gitlab = "gitlab id"
  twitter = "twitter id"
  linkedin = "linkedin id"
  email = "myemail"
  theme_colors = "color-dark"
~~~~

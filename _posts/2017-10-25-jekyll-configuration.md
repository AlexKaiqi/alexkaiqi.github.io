---
layout: post
title: Jekyll Configuration
date: 2017-10-25 21:23:22
categories: note jekyll configuration
tags: jekyll configuration
---
{% highlight yaml %}
defaults: # default configuration for sites
  -
    scope:
      path: "_posts"
      type: "posts"
    values:
      layout: "post"
  -
    scope:
      path: "_pages"
      type: "pages"
    values:
      layout: "page"
{% endhighlight %}

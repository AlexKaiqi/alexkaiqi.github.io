---
layout: page
title: About
categories: page about
tags: about
permalink: /about/
---

About content goes here.


### contacts
{% for page in site.contact %}{% if page.title %}
<li><a href="{{ page.url | prepend: site.baseurl }}">{{ page.title }}</a></li>
{% endif %}{% endfor %}

### blogs
{% for page in site.blog %}{% if page.title %}
<li><a href="{{ page.url | prepend: site.baseurl }}">{{ page.title }}</a></li>
{% endif %}{% endfor %}

### 2017
{% for page in site.posts %}{% if page.title %}
<li><a href="{{ page.url | prepend: site.baseurl }}">{{ page.title }}</a></li>
{% endif %}{% endfor %}

### jekyll update
{% for page in site.jekyll.update %}{% if page.title %}
<li><a href="{{ page.url | prepend: site.baseurl }}">{{ page.title }}</a></li>
{% endif %}{% endfor %}

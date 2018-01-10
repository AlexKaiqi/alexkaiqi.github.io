---
title: Jekyll Liquid
date: 2017-10-25 10:34:11
tags: jekyll liquid

my_defined_variable_name: my defined content
show_heading: true
capcakes:
  - chocolate
  - lemon
  - strawberry
---

## Liquid

Liquid is a templating language Jekyll uses to process pages on your site.
With Liquid you can output and modify variables,
have logic statements inside your pages and loop over content.

Let’s start with a basic example. We’ll add some content in front matter,
then output it using front matter.
Variables set in front matter are available to us at page.variable_name:


## There’s two tags in Liquid:

* We can output variables by surrounding them in two curly braces.
e.g.
```liquid
{% raw %}{{ variable }}{% endraw %}
```
* We can perform logic statements by surrounding them in a curly brace,
percentage sign e.g.
```liquid
{% raw %}{% if statement %}{% endraw %}
```
You can use your defined variable like this:
```liquid
{{ page.my_defined_variable_name }}
```


## Filters

We can run a variable through a filter to modify the output.
To use filter we'll add "|" after the variable the pass it a filter.
For example we want the output to be uppercase.
use <code>upcase</code> in this case:
```liquid
{{ page.my_defined_variable_name | upcase }}
```
We can run this content through multiple filters.
Here we’ll run in through a truncate to only output a maximum of eight characters:
```liquid
{% raw %}{{ page.variable_name | upcase | truncate: 8 }}{% endraw %}
```
```liquid
{{ page.my_defined_variable_name | upcase | truncate: 8 }}
```

## Logic Statements

Let’s control whether the h1 is output on the page.
We’ll add a new variable to the front matter called show_heading
and initalize it to true.
Then we’ll surround the h1 in an if statement to check if show_heading is true:
{% if page.show_heading %}
    ## {{ page.my_defined_variable_name | upcase }}
{% endif %}


## Loops

Let’s create a cupcakes array in front matter then loop over it
in Liquid and output it in an unordered list.
The syntax to loop in Liquid is for variable in array,
variable can named whatever you’d like and holds the item
in the current iteration of the loop:

```liquid
{% raw %}{% for page in site.pages %}{% endraw %}
Your Content
{% raw %}{% endfor %}{% endraw %}
```

{% for page in site.pages %}{% if page.title %}
* {{ page.title }}
   * {{ page.url }}
{% endif %}{% endfor %}


## syntax hightlight

Jekyll also offers powerful support for code snippets:

{% highlight liquid %}
{% raw %}{% highlight ruby %}{% endraw %}
{% endhighlight %}
{% highlight ruby %}
    def print_hi(name)
      puts "Hi, #{name}"
    end
    print_hi('Tom')
    #=> prints 'Hi, Tom' to STDOUT.
{% endhighlight %}
{% highlight liquid %}
{% raw %}{% endhighlight %}{% endraw %}
{% endhighlight %}


## Useful Resources

[supported language in jekyll](https://haisum.github.io/2014/11/07/jekyll-pygments-supported-highlighters/)
[Jekyll & Liquid cheatsheet](https://gist.github.com/smutnyleszek/9803727)

# Markdown
## Headers
# This is an h1 tag
## This is an h2 tag
###### This is an h6 tag

## Emphasis
*this text will be italic*
_this will also be italic_
**this text will be bold**
__this will also be bold__

## Lists
### Unordered
* Item 1
* Item 2
    * Item 2a
    * Item 2b
### Ordered
1. Item 1
2. Item 2
    1. Item 2a
    2. Item 2b
    
## Images
![Github Logo](https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "Logo Title Text 1")
## Links
[I'm an inline-style link](https://www.google.com)

http://github.com - automatic!

[I'm a relative reference to a repository file](../blog/index.html)

## Code
```javascript
var a = 0;
alert(a);
```
```python
s = "python syntax highlighting";
```

## Tables
name | age | gender
---|:---:|---:
tom | 20 | male
jerry | 21| male
sily | 22 | female

## Block Quotes
> This is a very long line that will still be quoted properly when it wraps. Oh boy let's keep writing to make sure this is long enough to actually wrap for everyone. Oh, you can *put* **Markdown** into a blockquote. 

> This is a short line

## Inner Html
<dl>
  <dt>Definition list</dt>
  <dd>Is something people use sometimes.</dd>
  <h3>paragragh</h3>
  <dt>Markdown in HTML</dt>
  <dd>Does *not* work **very** well. Use HTML <em>tags</em>.</dd>
</dl>

## Horizontal Rules
Three or more...
---
Hyphens
***
Asterisk
___
underscores

## Line Breaks
Here's a line for us to start with.

This line is separated from the one above by two newlines, so it will be a *separate paragraph*.

This line is also a separate paragraph, but...
This line is only separated by a single newline, so it's a separate line in the *same paragraph*.

# Github Flavored Markdown

```javascript
function fancyAlert(arg) {
  if(arg) {
    $.facebox({div:'#foo'})
  }
}
```
you can also simply indent your code by four space
    function fancyAlert(arg) {
      if(arg) {
        $.facebox({div:'#foo'})
      }
    }

Here’s an example of Python code without syntax highlighting:

def foo():
    if not bar:
        return True
        
## Task List
- [x] @mentions, #refs, [links](), **formatting**, and <del>tags</del> supported
- [x] list syntax required (any unordered or ordered list supported)
- [x] this is a complete item
- [ ] this is an incomplete item

## Tables
You can create tables by assembling a list of words and dividing them with hyphens - (for the first row), and then separating each column with a pipe |:

First Header | Second Header
------------ | -------------
Content from cell 1 | Content from cell 2
Content in the first column | Content in the second column

## SHA references
Any reference to a commit’s SHA-1 hash will be automatically converted into a link to that commit on GitHub.

16c999e8c71134401a78d4d46435517b2271d6ac
mojombo@16c999e8c71134401a78d4d46435517b2271d6ac
mojombo/github-flavored-markdown@16c999e8c71134401a78d4d46435517b2271d6ac

## Issue references within a repository
Any number that refers to an Issue or Pull Request will be automatically converted into a link.

#1
mojombo#1
mojombo/github-flavored-markdown#1

## Username @mentions
Typing an @ symbol, followed by a username, will notify that person to come and view the comment. This is called an “@mention”, because you’re mentioning the individual. You can also @mention teams within an organization.

## Automatic linking for URLs
Any URL (like http://www.github.com/) will be automatically converted into a clickable link.

## Strikethrough
Any word wrapped with two tildes (like ~~this~~) will appear crossed out.

## Emoji
GitHub supports emoji! :sparkles: :camel: :boom:

To see a list of every image we support, check out the [Emoji Cheat Sheet](https://www.webpagefx.com/tools/emoji-cheat-sheet/).
---
title: Markdown
nav: true
---

# Markdown *(in a few minutes)*

[Markdown](https://daringfireball.net/projects/markdown/) is a standard to simplify writing content for the web.
A handful of simple conventions translate into the basic HTML elements, making it quick to write and edit. 
Markdown can be used any where on GitHub, in popular static site generators such as Jekyll, and to create documents using Pandoc.

## Create a Markdown File

Create a new file in the repo:

- Click "Create new file" button on the repository page
- Type `about.md` in the name box
- Click into the editor
- Write some Markdown!
- Scroll to the bottom, add a message, and click *Commit new file*. (You just used Git again!)
- Behold lovely rendered Markdown on GitHub...

<button id="toggle" class="btn btn-success m-3">Toggle Markdown</button>

<div class="border p-3 mb-3">
<div id="source" markdown="1">

```
# Heading One

## Heading Two

### Heading Three, etc.

Any text with no empty lines between will become a paragraph.
Leave an empty line between headings and paragraphs.
Font can be *Italic* or **Bold**.
Code can be highlighted with `backticks`.

Hyperlinks look like this [GitHub Help](https://help.github.com/).
Images look similar:

![alt text here](https://upload.wikimedia.org/wikipedia/commons/4/4b/Focus_ubt.jpeg)

A bullet list is created using `*`, `+`, or `-`, like:

- dog
- cat
- muffin

A numbered list is created using a number + `.`, like:

1. one
2. two
6. three
2. four

----

```
</div>

<div id="rendered" markdown="1">

# Heading One

## Heading Two

### Heading Three, etc.

Any text with no empty lines between will become a paragraph.
Leave an empty line between headings and paragraphs.
Font can be *Italic* or **Bold**.
Code can be highlighted with `backticks`.

Hyperlinks look like this [GitHub Help](https://help.github.com/).
Images look similar:

![alt text here](https://upload.wikimedia.org/wikipedia/commons/4/4b/Focus_ubt.jpeg)

A bullet list is created using `*`, `+`, or `-`, like:

- dog
- cat
- muffin

A numbered list is created using a number + `.`, like:

1. one
2. two
6. three
2. four

----
</div>
</div>

## Jekyll?

Visit your `index.html` on your new site and click the link to `about.html`. 
Notice that your `about.md` has been converted into `about.html` and put in a fancy HTML template?

Behind the scene, gh-pages is running [Jekyll](https://jekyllrb.com/) static site generator. 
Jekyll automatically converted your Markdown into a lovely web page using a builtin theme.

## Resources

- GitHub Guide [Mastering Markdown](https://guides.github.com/features/mastering-markdown/)
- [GitHub markdown flavor](https://help.github.com/articles/basic-writing-and-formatting-syntax/) 
- [Dillinger](https://dillinger.io/) Markdown editor
- [Pandoc](https://pandoc.org/)

<script>
function markdownToggle() {
    document.getElementById("source").style.display = (document.getElementById("source").style.display === "none") ? "block" : "none";
    document.getElementById("rendered").style.display = (document.getElementById("rendered").style.display === "block") ? "none" : "block";
}
document.getElementById("rendered").style.display = "none";
document.getElementById("toggle").onclick = function () { markdownToggle(); };
</script>
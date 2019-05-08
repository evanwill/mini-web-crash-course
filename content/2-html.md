---
title: HTML
nav: true
---

# HTML *(in a few minutes)*

The web is made up of HTML, CSS, and JS (*mostly*).

- HTML provides the structure and content
- CSS provides the style
- JS provides the interactivity

When you access a website, the server sends your computer the code, and your browser renders it into a web page.
Thus, you have the code for every web page you visit on your machine.

Right click on any page and select "View page source" to check it out!

Or put `view-source:` in front of any URL.

{% include figure.html img="nicolas-picard-241854-unsplash.jpg" alt="spider web" width="65%" %}

## Hypertext Markup Language

HTML is a ["markup language"](https://en.wikipedia.org/wiki/Markup_language) originally designed to describe documents for the web.
HTML is made up of a set of standard **elements** used to structure a web page and introduce features such as images.
Elements are represented by **tags** using point brackets, `<tag></tag>`.

Every HTML file starts with the *doctype declaration* `<!DOCTYPE html>` which tells your web browser what type of file it is. 
Next comes the **root element** `<html>`. 
The rest of the web page is **nested** inside the root element, so the final tag on every HTML file will be `</html>`.

## Create a web page

Create a new repository on GitHub:

- Click the plus sign in the upper right
- Select "New repository"
- Give your repo a unique name (no spaces please!)
- Check "Initialize this repository with a README"
- Click green "Create repository" button

Create a new file in the repo:

- Click "Create new file" button on the repository page
- Type `index.html` in the name box
- Click into the editor
- Write some HTML!
- Scroll to the bottom, add a message, and click *Commit new file*. (You just used Git!)

Our basic page:

```
<!DOCTYPE html>
<html>
    <head>
        <title>Hello!</title>
    </head>
    <body>
        <h1>Hello World!</h1>
        <p>gh-pages rock!</p>
        <p>See <a href="about.html">About page</a></p>
    </body>
</html>
```

Activate GitHub Pages:

- Click on the repository's *Settings* tab.
- Scroll down to the *GitHub Pages* options.
- Click *Source*, select *Master branch*, and click *Save*. 
- Wait for a minute for gh-pages to build. The live link will appear in the options.

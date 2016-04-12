---
title: How To
layout: template
--- 

# How to Create a Multi-page Website using Github Pages

### To Create the Template
1. Create the page normally following [pages.github.com](https://pages.github.com), but use `CONTENT` as the content of the page
2. Choose a theme and publish the page
3. Fetch and checkout the gh-pages branch on your local repository
4. Create a directory `_layouts` in the repository
5. Rename `index.html` to `template.html` and move it into the `_layouts` directory
6. Open `template.html` and replace the `<p>CONTENT</p>` placeholder with `{{ content }}` (this is [Jekyll](https://jekyllrb.com) syntax to grab the content from the MarkDown pages you will create)

### To Create Your First Page
1. Make a new file called `index.md` in your repository
2. Copy the content of your `readme.md` or write a new home page in MarkDown into this file
3. At the top of this file, add the following:
```
---
title: PAGE TITLE HERE
layout: template
--- 
```
4. Commit your changes and push them to the gh-pages branch

Now, when you go to `YOURGITHUBNAME.github.io/YOURPROJECTNAME`, you should see the contents of your index.md formatted with the theme that you chose

### To Create Additional Pages
1. In template.html, identify the navigation/button section of code 
2. For each additional page you add, create a new button or link, but replace
1. Make a new file called `PAGENAME.md` in your repository (where PAGENAME is the name of your page)
2. Write the content for the new page in MarkDown
3. At the top of this file, add the following:
```
---
title: PAGE TITLE HERE
layout: template
link: index
--- 
```
4. To link to this page from 
4. Commit your changes and push them to the gh-pages branch
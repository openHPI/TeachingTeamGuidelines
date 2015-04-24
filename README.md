# TeachingTeamGuidelines
This GitHub repository contains markdown files for building up an online documentation for the Xikolo MOOC platform with ReadTheDocs. Here the basics about how it works is summed up.

## General Info

A way of putting a documentation online is the combination of three tools:

- **GitHub**

Can be used for hosting and editing the necessary files representing the documentations content (the markdown files) and structure (.yml file)

- **MkDocs**

This is essentially a python script, i.e. the technology used to build static html files as the output; takes the markdown files and the one .yml configuration file as input.

- **ReadTheDocs**

A webservice using MkDocs as one backend for building the documentation out of markdown files and hosting the html documentation site in the end; it connects to GitHub (or other sources) to read in the content (markdown files) and configuration (mkdocs.yml file)

## Updating the Teaching Guidelines
### 1st step: Editing Process

- Log in here on GitHub, make sure you have owner status for this repository and
- **add/edit markdown file(s)** to update the content of the documentation
- if you want to reorder chapters or add new md-files, edit the *mkdocs.yml* and adjust order/filenames
- *also* adjust those changes inside the *index.md* file
- CAVE: **but never rename the mkdocs.yml or the index.md files**!
- you can also customize themes and build more complex document structures (follow the link to the manuals below)

![.yml configuration file](/docs/pics/readme_screenshot.png)

### 2nd step: Building Process

- Log in at [--> ReadTheDocs](https:/readthedocs.org)
- **make a new build**. ReadTheDocs will fetch the files from GitHub and update the documentary immediately. For more info about this process look up the ReadTheDocs documentation (link below).

![rtd environment](/docs/pics/readme_screenshot-2.png)


## More info ...
... about ReadTheDocs:

 - [ReadTheDocs Manual](http://read-the-docs.readthedocs.org/en/latest/)
 - [RTD GitHub Page](https://github.com/rtfd/readthedocs.org)
 
... about MKDocs (the python backand ReadTheDocs is using to build an HTML site out of md-files):

 - [MkDocs Manual](http://www.mkdocs.org/)
 - ["Documenting your project with MkDocs"](https://ep2014.europython.eu/de/schedule/sessions/39/): Video by the developer Tom Christie

... about Markdown

 - Syntax Documentation on [Daring Fireball](http://daringfireball.net/projects/markdown/syntax)
 - [Editor MarkdownPad2](http://markdownpad.com/) (if you feel more comfortable with editing on your local system and syncing with GitHub afterwards)
 
 

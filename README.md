# TeachingTeamGuidelines
This repository contains markdown files for building up a documentation with ReadTheDocs

## General Info

A way of putting a documentation online is the combination of three tools:

### GitHub

Can be used for hosting and editing the necessary files representing the documentations content (the markdown files) and structure (.yml file)

### MkDocs

This is essentially a python script, i.e. the technology used to build static html files as the output; takes the markdown files and the one .yml configuration file as input.

### ReadTheDocs

Is using MkDocs for building and hosting the documentation in the end; it connects to GitHub (or other sources) to read in the content (markdown files) and configuration (mkdocs.yml file)


## More info ...

... about MKDocs:

 - [MKDocs-Website](http://www.mkdocs.org/)
 - ["Documenting your project with MkDocs"](https://ep2014.europython.eu/de/schedule/sessions/39/): Video by the developer Tom Christie
 

... about ReadTheDocs:

 - [GitHub-Page](https://github.com/rtfd/readthedocs.org)
 - [ReadTheDocs at ReadTheDocs](http://read-the-docs.readthedocs.org/en/latest/)
 
 
## Updating the Teaching Guidelines

Log in here on GitHub and
- **edit markdown file(s)** to update the content
- if necessary: edit the *mkdocs.yml* file in this repository for reordering of the chapters, after adding new chapters

Log in at [ReadTheDocs](https:/readthedocs.org) and **make a new build**. ReadTheDocs will fetch the files from GitHub and update the documentary immediately. For more info about how this works with read the docs look the ReadTheDocs link above and choose chapter 'build'.

**CAVE:** You must not rename the file *index.md* in the docs folder since ReadTheDocs/mkDocs needs this file named this way. In case of renaming the other markdown files with the documentation content make sure to also adjust these changes inside the mkdocs.yml file (the file which determines the structure/order for the files appearing in the documentation).

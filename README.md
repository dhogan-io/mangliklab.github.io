mangliklab.github.io
====================

Getting started
---------------

 1. Install all [prerequisites](https://jekyllrb.com/docs/installation/)
 1. Install the jekyll and bundler gems
    ```
    gem install jekyll bundler
    ```
 1. Clone this repository
    ```
    git clone git@github.com:mangliklab/mangliklab.github.io.git
    ```
 1. Change into your new directory
    ```
    cd mangliklab.github.io
    ```
 1. Build the site and make it available on a local server
    ```
    bundle exec jekyll serve
    ```
 1. Browse to `http://localhost:4000`

Please test your changes locally before pushing.

Basic repository layout
-----------------------
```
.
├── assets/
│   ├── css/
│   │   └── main.scss #used to increase the maximum width of text
│   │                 #hurts readability but uses screen more efficiently
│   └── images/ #avoid anything over 1 MB unless necessary
│       ├── last-first.jpg #member headshots; aim for 500x500 px JPGs at <200 KB
│       └── schematic.png
├── \_config.yml #set global site properties
├── \_data/
│   ├── authors.yml #list of possible post authors; generates sidebar of post
│   │               #also used to generate member page in listed order
│   └── navigation.yml #sets the categories in the page headers
├── favicon.ico #the small square icon in the tab bar; ideally 256x256 px PNG
│               #browser caching behavior of favicons can be weird
├── Gemfile
├── Gemfile.lock #ignore; autogenerated by jekyll
├── .git/ #stores repo information, history, and branches
├── .gitignore #list of files that git shouldn't monitor
│              #generally, this should only include files you make
├── index.html #front page of the website
├── \_pages/ #creates various pages
│   ├── 404.md #creates the page displayed when the URL doesn't exist
│   ├── about.md
│   ├── category-archive.md
│   ├── members.md
│   ├── publications.md
│   ├── research.md
│   ├── tag-archive.md
│   └── year-archive.md
├── \_posts/ #each entry generates a post; some also generate a publication
│   │        #add "publication=true" to the front matter for publications
│   │        #files must be YYYY-MM-DD-short-summary.md; used to generate URL
│   ├── 2020-01-01-new-website.md
│   └── 2021-01-01-publication-1.md
├── README.md #this file
├── \_research/ #each file in this dir creates a section on the research page
│   ├── interest-1.md
│   └── interest-2.md
└── \_site #do not edit; autogenerated by jekyll's processing of the above
```
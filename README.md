# St. Gallen Methods Reading Group

This is the website for the _St. Gallen Methods Reading Group_:

__[🔗hsg-methods-reading-group.github.io](https://hsg-methods-reading-group.github.io)__

## Requirements to Edit

This website is built using Zola (https://www.getzola.org/), a static website generator. 
Please note that you need to install Zola before updating the website.
For a basic intro to Zola, go to

https://www.getzola.org/documentation/getting-started/overview/

## Site Structure
* Folder `content` contains the main pages of the website in Markdown format.

* For each edition (semester/year/topic), please create a new file in the  folder `content/editions` named according to the expression `YEAR_SEMESTER.md` such that
    + `YEAR`: four-digit year
    + `SEMESTER`: semester of the academic year 
    + __IMPORTANT:__ In the head section of the `md` file (wrapped by `+++ ... +++`) please include the field `description = "XX"`, where `XX` is a two-digit number (including a zero first for single-digit numbers) that is increasing in the edition of the group. _This enables the website to be correctly compiled and always show the most recent edition as front page._

* To update general info, change `content/about.md`

* File `past-editions.md` is *automatically updated at site build time*: __do not edit this file unless you know what your are doing!__

__Important:__ files `_index.md` are needed internall by Zola, please do not edit them.

## Local Work on the Website

__Note:__ this repository is set up so that anytime a _push_ is detected, a Github Action will
automatically re-compile the website and push it to the `gh-pages` branch. <br>
*Please **do not** push directly to branch `gh-pages` by hand!*

To locally build & update the site: clone the repo, open a terminal at the root of the repo and run

> zola serve

A local webserver should be available at the local address `127.0.0.1:1111`


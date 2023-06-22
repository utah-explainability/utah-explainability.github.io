# Computational Ethics in NLP Website

This is the source code for the course website for
[CSE 599D1: Computational Ethics in NLP](https://courses.cs.washington.edu/courses/cse599d1/22wi/),
held in Winter 2022.

It is a [Jekyll](https://jekyllrb.com) site based on a few modifications to
the [Just the Class](https://github.com/kevinlin1/just-the-class) template,
which is itself built on the
[Just the Docs](https://github.com/pmarsceill/just-the-docs) theme.
See those repositories for details on their structure and features.

## Usage

We are hosting the site using the UW CSE course website webserver, which statically serves documents
from the CS UNIX machines. Continuous integration has been set up so that updates pushed to the
`main` branch of this repository get automatically copied to the webserver.

To preview the site locally, make sure ruby is installed, then run `bundle exec jekyll serve` from
the base directory of the repository. Then you can see the site at
[`localhost:4000/courses/cse599d1/22wi/`](localhost:4000/courses/cse599d1/22wi/).
See
[Setting up your GitHub Pages site locally with Jekyll](https://help.github.com/en/articles/setting-up-your-github-pages-site-locally-with-jekyll)
for more details.

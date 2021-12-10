# FP Optik
 Introduction to the FP Optik.

 You can:

 - read it [on the website](https://synqs.github.io/FP-Optik/intro.html).
 - download the book as [pdf](book.pdf)
 - report issues in the [issue tracker](https://github.com/synqs/FP-Optik/issues).
 - provide improvements to the manuscript through modifications in the markdown files.
 - just enjoy that you are learning optics.


## How-to make changes

The tutorial is based on [jupyter-books](https://jupyterbook.org/intro.html).

Here are the typical steps to make changes:

- clone this repository to your local PC.
- go into the directory folder.
- install the necessary requirements through `pipenv install`
- make changes in the appropriate markdown file. They are all located in the `tutorial` folder.
- run `pipenv run jupyter-book build tutorial` once you are in the git folder to create the website.
- You can look at your book by opening this file in a browser: *tutorial/_build/html/index.html*

## Publish changes to the github pages

- push the changes through `pipenv run ghp-import -n -p -f tutorial/\_build/html`.

## Create a book.pdf

- make sure that you have a running latex environment
- run `pipenv jupyter-book build tutorial/ --builder pdflatex`from the root directory.
- copy the *book.pdf* file that is created in *tutorial/\_build/latex* into the root directory.
- push the changes.

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
- Install jupyter-book through `pip install -U jupyter-book`
- make changes in the appropriate markdown file. They are all located in the `tutorial` folder.
- run `jupyter-book build tutorial` once you are in the git folder to create the website.
- You can look at your book by opening this file in a browser: *tutorial/\_build/html/index.html*
- Delete the *\_build* directory once you are done with the changes.

## Publish changes to the github pages

- Pip install the *ghp-import* package through `pip install ghp-import`.
- Run `jupyter-book build tutorial` to create the website files.
- Change the directory into *tutorial* folder through `cd tutorial`.
- push the changes through `ghp-import -n -p -f _build/html`.
- remove the changes to the `_build` directory again.

## Create a book.pdf

- make sure that you have a running latex environment
- run `jupyter-book build tutorial/ --builder pdflatex`from the root directory.
- copy the *book.pdf* file that is created in *tutorial/\_build/latex* into the root directory.
- remove the folder that was created in *tutorial\_build*
- push the changes.

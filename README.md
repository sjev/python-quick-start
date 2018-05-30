# Python quick start
Example project for creating a module with a good structure, documentation and testing 


The `conf.py` file has been generated with `sphinx-autostart` and then edited by hand.



**Additions and comments are welcome!**

## Resources
* [Sample Doc](http://matplotlib.org/sampledoc/cheatsheet.html) Quick example of rst usage
* [RST primer](http://www.sphinx-doc.org/en/stable/rest.html) More extensive primer of rst synthax
* [numpy style guide](https://github.com/numpy/numpy/blob/master/doc/HOWTO_DOCUMENT.rst.txt)
* [pandas docs](http://pandas.pydata.org/pandas-docs/version/0.17.1/) An excellent piece of example documentation. The theme was borrowed from that project.


## Building docs
1. install `numpydoc` sphinx extension first ( `pip install numpydoc`)
2. run `make html` in the `doc` folder

## Publishing on github pages

The pages can be published on github, either on a special branch named `gh-pages` or in a subfolder `docs` on the main branch.
Using `docs` folder is the most convenient approach.

1. create `docs` folder and use it as a target for sphinx build.
2. create a `.nojekyll` file, otherwise pages and directories starting with underscore will be ignored
3. build and commit the docs

The docs for this project are published [here](http://sjev.github.io/numpy-sphinx-example).

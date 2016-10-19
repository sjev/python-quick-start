# numpy-sphinx-example
Example project for documenting with sphinx numpy-style

This example project is a reference on how to create sphinx documentation.
The source code resides in `lib` directory, the docs in `doc` directory.

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

The pages can be published on a special `gh-pages` branch, where `index.html` must be in the root.

1. checkout the `master` branch to a *separate* folder, create a new clean branch

```
git branch gh-pages
git checkout gh-pages
git symbolic-ref HEAD refs/heads/gh-pages
rm .git/index
git clean -fdx
```

2. build the docs
3. copy biult docs to the location of `gh-pages` branch, add files, commit and push. 

The docs for this project are published [here](http://sjev.github.io/numpy-sphinx-example).

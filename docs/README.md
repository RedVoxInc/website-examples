# How to contribute to the RedVox Website Examples Docs

### Python libraries required

- sphinx
- furo, the sphinx theme used
- myst-parser, to parse markdown (.md) files to sphinx

Note: `requirements_docs.txt` in the `docs` folder is the requirements used by the Github action in 
.github/workflows/docs_gh_pages.yml to construct the docs and push to the branch `gh-pages`. 
Please do not change/move.

### Editing the docs

The meat of the documentation is in `website-examples/docs/source`. The `.md` files are the base of the documentation.
You also need the conf.py file to be in the source directory.

If you add new `.md` files, make sure that `index.rst` inside the `source` folder points to the new file using
`.. toctree::`.

Please do not modify the following files in the `docs` folder (unless you really know what you are doing):
- `.nojekyll` - used for hosting the docs in Github Pages
- `make.bat` and `Makefile` - used by sphinx to clean and build the documentation
- `index.html` inside the `docs` folder (okay to modify the `index.rst` inside the `source` folder) - used for hosting 
the docs in Github pages
- `requirements_docs.txt` - used by Github actions

### Viewing the docs locally

Once you are done with your changes, open a terminal with a python environment, cd to datawindow-examples/docs, and type `make clean` and `make html`.
`make clean` will eliminate everything in the `build` folder and `make html` will (re)build the documentation.

```shell
(venv3910) user@comp website-examples % cd docs
(venv3910) user@comp docs % make clean 
(venv3910) user@comp docs % make html 
```

To view the docs in a browser, go to website-examples/docs/build/html and open `index.html` in a browser.

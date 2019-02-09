# Contributing

At CoderDojoKC, we would like to provide a nice way for the community to help improve our lessons.

## Code of Conduct

We follow the [CoderDojo Charter](https://zen.coderdojo.com/charter) and adhere to the [Kansas City Women in Technology Code of Conduct](https://kansascitywomenintechnology.github.io/CodeOfConduct/)

## Text Markup

This project uses two different kinds of text markup:

* [markdown](https://daringfireball.net/projects/markdown/)
* [restructuredText](http://docutils.sourceforge.net/rst.html)

If you're writing something without images or tables, you can use markdown. It provides an easy and quick way to create formatted text with lists and nicely formatted code examples. A good [markdown cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)

If you're writing something with images or tables, please write it using restructuredText. RestructuredText uses a semantic markup that allows one to create accessible documentation. For instance, if you have an image that requires a licensing notice or a citation, you can more easily create a [caption in restructuredText](https://thomas-cokelaer.info/tutorials/sphinx/rest_syntax.html#images-and-figures) than you can in markdown. A good [restructuredText cheatsheet](https://thomas-cokelaer.info/tutorials/sphinx/rest_syntax.html)

## Building a local version

### Requirements

* Python 3
* [pipenv](https://pipenv.readthedocs.io/en/latest/install/#installing-pipenv)

### How to

**Get Started:**

1. Fork this repository
1. Clone this repository to your local development machine: `git clone <your-fork.git>`
1. CD into the directory the new directory: `cd !$`
1. Install the python dependencies and enter the virtual environment just for this project: `make dev`

**To build an HTML version of this documentation locally:**

1. `make html`
1. Open `build/html/index.html` in your favorite browser

**To add a python package:**

1. `pipenv install (--dev) name-of-package`
1. `make requirements` to add it to the `requirements.txt` or `requirements-dv.txt` file

// todo Making a Pull Request

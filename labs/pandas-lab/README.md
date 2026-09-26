# Pandas Lab

A maintained edition of Brandon Rhodes’s **Pandas From The Ground Up**, originally presented at PyCon 2015.

Original work © 2015 Brandon Rhodes, licensed under the MIT License. This edition updates the tutorial for modern Python and pandas while preserving the original teaching progression and exercises.

Maintained by Scott Halkyard.

## Quick Start

If you have both `uv` and `git` installed:

```bash
git clone https://github.com/halkypi/pandas-lab.git
cd pandas-lab

bash requirements.sh
source .venv/bin/activate

build/BUILD.sh
jupyter notebook
```

Validated with Python 3.13.12 and pandas 3.0.6.

## Detailed Instructions

You will need Pandas, Jupyter Notebook, and Matplotlib installed before you can successfully run the tutorial notebooks.

Git is not required. You can also download the repository as a ZIP archive from GitHub.

The tutorial uses the original frozen IMDb data files:

* `actors.list.gz`
* `actresses.list.gz`
* `genres.list.gz`
* `release-dates.list.gz`

The validated source is:

https://www.nic.funet.fi/pub/mirrors/ftp.imdb.com/pub/frozendata/

The build script downloads and prepares the data:

```bash
build/BUILD.sh
```

Or, if the archives are already in `build/`:

```bash
python build/BUILD.py
```

Then start Jupyter:

```bash
jupyter notebook
```

## Tutorial Notes

The numbered solution notebooks are the teaching sources for the numbered exercises.

`build/split.py` regenerates the exercises from the solutions; run it only when intentionally updating exercises.

`All.ipynb` is an older exploratory collection.

`images/Diagrams.ipynb` is auxiliary material and should be run from `images/`.

## Original Tutorial

Brandon Rhodes’s original repository:

https://github.com/brandon-rhodes/pycon-pandas-tutorial

PyCon 2015 tutorial:

https://www.youtube.com/watch?v=5JnMutdy6Fw

## License

MIT License. See `LICENSE.txt`.

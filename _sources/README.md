# AMAAI-guidebook

This is the source code for the guidebook.

The html version of this guidebook is assessible at:

https://amaai-lab.github.io/AMAAI-guidebook/docs/index.html

## Compiling
First make sure `jupyter-book` is installed. If not, it can be installed using:
```bash
pip install -U jupyter-book
```

To build the book, go to the root of this repo, and do 
```bash
jupyter-book build ./
```

After that, a new folder called `_build` will appear. The html files for the book are located inside this folder.

If the built book does not reflect the lastest version of the source code, you should remove the old contents in the `_build` folder. Alternatively you can do:
```bash
jupyter-book clean ./
```

## Modifiying the cotents
The contents of the jupyter book are inside the `docs` folder.

The book layout is defined in `_toc.yml`.

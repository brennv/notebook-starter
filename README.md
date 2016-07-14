# notebook-starter

For getting started with Python notebooks

- [Getting started](https://github.com/brennv/notebook-starter#getting-started)
- [Example notebooks](https://github.com/brennv/notebook-starter#example-notebooks)
- [Clean up](https://github.com/brennv/notebook-starter#clean-up)

## Getting started

Install [Docker](http://www.docker.com/products/docker), open [Terminal](http://blog.teamtreehouse.com/introduction-to-the-mac-os-x-command-line) and run:

    docker run -p 8888:8888 -v ~/projects/scipy-notebooks:/home/jovyan/work \
        jupyter/scipy-notebook start-notebook.sh --NotebookApp.base_url=/home/jovyan/work

This will create or sync folders `~/projects/scipy-notebooks` and start a [jupyter notebook](http://www.jupyter.org) with Python 3 and some scientific packages installed.

If this is the first time you're running it, go get a coffee and check out these [ipython notebooks](https://github.com/ipython/ipython/wiki/A-gallery-of-interesting-IPython-Notebooks#introductory-tutorials) for inspiration.

Optionally, add some csv or excel files to the folder `~/projects/scipy-notebooks` to play with later.

Once jupyter is running you'll see something like:

    [NotebookApp] The Jupyter Notebook is running at...
    [NotebookApp] Use Control-C to stop this server and shut down all kernels.

Now grab your browser and go to [http://localhost:8888](http://localhost:8888)

## Example notebooks

See the (in-progress) [examples/](https://github.com/brennv/notebook-starter/tree/master/examples) folder and check out these notebook galleries:

- [ipython](https://github.com/ipython/ipython/wiki/A-gallery-of-interesting-IPython-Notebooks#introductory-tutorials)
- [bianp](http://nb.bianp.net/sort/views/)
- [wakari](https://wakari.io/gallery)

Also:
- [Common excel tasks in Pandas](http://pbpython.com/excel-pandas-comp.html)
- [vlookup in Pandas](http://stackoverflow.com/questions/25493625/vlookup-in-pandas-using-join)
- [Pandas docs](http://pandas.pydata.org/pandas-docs/stable/index.html)
- [devnami tutorial videos](https://www.youtube.com/user/devnami/search?query=notebook)

## Clean up

When you're done, head back to the terminal and hit Control-C. 

If you like, delete the `projects/scipy-notebooks` folders.

## Attributions

Built on top of [jupyter/docker-stacks](https://github.com/jupyter/docker-stacks)

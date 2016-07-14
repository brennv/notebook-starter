# notebook-starter

For getting started with Python notebooks

## Getting started

Install [Docker](http://www.docker.com/products/docker), open Terminal and run:

    docker run -p 8888:8888 -v ~/projects/scipy-notebooks:/home/jovyan/work \
        jupyter/scipy-notebook start-notebook.sh \
        --NotebookApp.base_url=/home/jovyan/work

This will create or sync folders `~/projects/scipy-notebooks` and start a [jupyter notebook](http://www.jupyter.org) with Python 3 and some scientific packages installed.

If this is the first time you're running it, go get a coffee and check out these [ipython notebooks](https://github.com/ipython/ipython/wiki/A-gallery-of-interesting-IPython-Notebooks#introductory-tutorials) for inspiration.

Optionally, add some csv or excel files to your new folder to play with later.

Once jupyter is running you'll see something like:

    [NotebookApp] The Jupyter Notebook is running at...
    [NotebookApp] Use Control-C to stop this server and shut down all kernels.

Now grab your browser and go to [http://localhost:8888](http://localhost:8888)

## Clean up

When you're done, head back to the terminal and hit Control-C.

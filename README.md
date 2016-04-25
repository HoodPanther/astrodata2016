# astrodata2016
Notebook for Astropy class at IPAC held in April 2016.

Click on the .ipynb link below for a rendered version.

## Launching an interactive instance

[![Binder](http://mybinder.org/badge.svg)](http://mybinder.org/repo/stargaser/astrodata2016)

## Installation of Python modules
If you don't have Anaconda or Miniconda, go to http://conda.pydata.org/miniconda.html and install the Python 3.5 64-bit version for your system. 

Make sure you've added the `bin` directory for Miniconda to your `PATH`. Then in a terminal window, execute this command:
```
conda create -n course python=3.5 astropy pandas seaborn glueviz jupyter pillow
```
This creates a virtual environment named `course`. You can list your environments with `conda info -e`.

### Activate the virtual environment

In a bash-like shell:
```
source activate course
```

In a csh-like shell, the `activate` is not available. Look at the output of `conda info -e` for the path to your `course`
virtual environment. Then add it to your PATH environment variable. Or, use this UNIX one-liner:
```
setenv PATH `conda info -e | grep course | awk '{printf("%s/bin\n",$NF)}'`:$PATH
```

### Install packages not available in conda

From your `course` virtual environment, install these additional packages:

```
pip install astroquery
pip install photutils
pip install aplpy
pip install ginga
```

## Starting the notebook
Either `git clone` the repository, or click on `Download ZIP` and unpack the zip file.

Activate your virtual environment as above. Then, in the directory where the `.ipynb` file resides, do:
```
jupyter notebook
```

A web browser will pop up. You can start the notebook by clicking on its link.

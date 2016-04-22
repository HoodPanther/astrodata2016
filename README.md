# astrodata2016
Notebook for Astropy class at IPAC held in April 2016.

## Installation of Python modules
If you don't have Anaconda or Miniconda, go to http://conda.pydata.org/miniconda.html and install the Python 3.5 64-bit version for your system.

Then in a terminal window, execute these commands:
```
conda create -n course python=3.5 astropy pandas seaborn glueviz jupyter pillow
source activate course
pip install astroquery
pip install photutils
pip install aplpy
pip install ginga
```

## Starting the notebook
Either `git clone` the repository, or click on `Download ZIP` and unpack the zip file.

Then, in the directory where the `.ipynb` file resides, do:
```
source activate course
jupyter notebook
```

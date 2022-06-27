# Installing Python

stall the latest version of Anaconda Python version 3.x .  Please verify that you can run Python version 3, and that you can open a Jupyter notebook with Python 3.  One way to do this is to use the Navigator that is installed with Anaconda (the icon looks like a green ring), and then click on the Jupyter notebook box within the navigator.  If you already have Python 3 installed and working, with Jupyter notebooks available, you can probably skip this step. (Though I strongly recommend Anaconda Python over whatever default comes installed on your machine; see below for one important reason.)  If you are installing Anaconda on Windows, I recommend checking the option to add Anaconda to your Windows PATH – this will allow you to easily run Python through your Bash terminal just like on Mac or Linux.

## Setting up a new Python environment in Anaconda

One of the major advantages to using Anaconda Python is that it allows you to create multiple Python “environments” on your computer.  For instance, if you want to install some Python package but are worried it might corrupt your Python install, or if you usually use Python 2.7, but now you need Python 3.10, environments are the solution you’ve been looking for.  Here’s some documentation that may be useful, and below I will write the specific commands that you should type in your bash terminal to create your environment for this REU program.   (If you can’t get these to work before the summer, that’s OK.  I will help during our first Python workshop.)

To create your REU2022 Python environment (command should be all one line):

```
conda create -n REU2022 -c conda-forge python=3.10 jupyter numpy scipy matplotlib pandas astropy astroquery bokeh emcee corner
```

To activate this environment (do this before running any Python commands):

```
conda activate REU2022
```

To deactivate this environment (and return to your default Python):

```
conda deactivate
```

# Poseidon Bot

[![Binder](https://binder.pangeo.io/badge_logo.svg)](https://binder.pangeo.io/v2/gh/rabernat/poseidon-bot/master)
![Twitter Follow](https://img.shields.io/twitter/follow/llc4320bot)

This is a bot that tweets out images of the MITgcm LLC4320 ocean simulations.

The code is open source (MIT License).

The images produced by the bot are licensed under a
[Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/).

### Simulation Credit

These simulations were produced by Dimitris Menemenlis (JPL) and Chris Hill (MIT)
using the NASA Pleaiades Supercomputer.
See [this talk by Dimitris](http://online.kitp.ucsb.edu/online/blayers18/menemenlis/pdf/Menemenlis_BLayers18_KITP.pdf) for more information.

### The Data

The data are stored in Google Cloud in the [Zarr](https://zarr.readthedocs.io/) format.
They are available via the [Pangeo Cloud Data Catalog](https://catalog.pangeo.io/browse/master/ocean/LLC4320/)

### Software Used

This bot is a Jupyter notebook. It uses open source Scientific Python packages, including
- [Xarray](http://xarray.pydata.org/): the central data model and computational library
- [XGCM](https://xgcm.readthedocs.io/en/latest/) for grid-aware operations (e.g. calculating vorticity)
- [Matplotlib](https://matplotlib.org/) and [Cartopy](http://scitools.org.uk/cartopy/index.html) for plotting
- [Zarr](https://zarr.readthedocs.io/), [gcsfs](https://gcsfs.readthedocs.io/), and [intake](https://intake.readthedocs.io/) for data storage and cataloging

### Automation

The bot is automated using github workflows and [binderbot](https://github.com/pangeo-gallery/binderbot/).

You can run the code yourself by following the Binder link above.

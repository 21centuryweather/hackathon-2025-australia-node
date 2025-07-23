# Kilometre-Scale Global Hackathon 2025

This repository includes the instructions to meet all the technical requirements to work during the Hackathon. It also includes examples on how to work with `healpy` and the helpix grid. 

### 1. Join the neccesary NCI projects

Please log in into [my.nci.org.au](https://my.nci.org.au/mancini/) and join the following projects:

* `qx55` (where the km-scale simulations live. Check [the available simulations here](/available_simulations.md))
* `xp65` (to access the conda environment, see below)
* and any other project you think you will need. For example, join `rt52` if you are going to use ERA5 data.

### 2. Clone this repository 

If you want to run the examples located in `notebooks/` clone this repository in Gadi (to be able to access the **test data**).

```
git clone git@github.com:21centuryweather/hackathon-2025-australia-node.git
```
### 3. Conda environment

To process the hackathon data, we need some extra python modules that aren't included in the standard `xp65` analysis3 conda environment. So a python virtual environment has been created to use for the hackathon. To use it, load the `xp65` conda environment as normal, but take care to load a specific version of analysis3:
```
module use /g/data/hh5/public/modules
module load conda/analysis3-25.02
```
Now type the following to load the virtual environment.
```
source /g/data/gb02/public/venvs/hackathon_env/bin/activate
```
This should modify your gadi login prompt to
```
(hackathon_env) [<user-id>@gadi-login-0<username> ]$
```
You can test this virtual environment can load our required modules form the command line using python or ipython
```
$ python
Python 3.11.11 | packaged by conda-forge | (main, Dec  5 2024, 14:17:24) [GCC 13.3.0] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> import healpy as hp
>>> import easygems.healpix as egh
```
To use the correct version of `ipython`, type `python -m IPython`.
```
$ python -m IPython
Python 3.11.11 | packaged by conda-forge | (main, Dec  5 2024, 14:17:24) [GCC 13.3.0]
Type 'copyright', 'credits' or 'license' for more information
IPython 9.4.0 -- An enhanced Interactive Python. Type '?' for help.
Tip: You can find how to type a Unicode symbol by back-completing it, eg `\Ⅷ<tab>` will expand to `\ROMAN NUMERAL EIGHT`.

In [1]: import healpy as hp

In [2]: import easygems.healpix as egh
```

To use this environment in an ARE session, link the juypyter kernel to your local directory.
```
mkdir -p ~/.local/share/jupyter/kernels/
cd ~/.local/share/jupyter/kernels/
ln -s /g/data/gb02/public/venvs/hackathon_env/share/jupyter/kernels/hackathon_env/
```
Start an ARE session with the storage parameters you need. Make sure to include
* gdata/qx55 (where the km-scale simulations live)
* gdata/xp65 (to load the python analysis3 interpreter)
* gdata/gb02 (to load the hackathon virtual environment)

in addition to other storage fields you will require for your work (e.g. gdata/rt52 if you use ERA5 data).

<img src="images/ARE_project_storage.png" style="width:50%; height:auto;">

Now click on the **advanced settings:**

<img src="images/ARE_advanced_settings.png" style="width:50%; height:auto;">

Specify the **Module** directories and **Modules** fields as set out below.

> [!NOTE] 
> This is slightly different to loading other conda environments into the ARE you may have used previously.

Use the following **advanced options:**

<img src="images/ARE_advanced_options.png" style="width:50%; height:auto;">

When the ARE session has loaded, make sure to check the Jupyter path points to the xp65 analysis3-25.0.2d directory.

<img src="images/ARE_session.png" style="width:50%; height:auto;">

Inside the notebook, click on the kernel selection pull down menu in the top right corner.

<img src="images/ARE_kernel_select.png" style="width:50%; height:auto;">

Of the available options (and yours may differ), select 'hackathon_kernal'

<img src="images/ARE_kernel_pulldown.png" style="width:50%; height:auto;">

Happy coding!

## Projects 

Here is the list of projects proposed by the Australian node. We encourage you to check them but also visit the [global hackathon website](https://digital-earths-global-hackathon.github.io/hk25/) to find other relevant projects and people working on similar topics. 

* Towards enhancing climate projections through improved understanding and simulations of marine low clouds
* [Evaluation of Meso-scale Degree of Organization of Convection](https://github.com/21centuryweather/hk25-AusNode-DOCmeso)
* [Chasing Cyclones](https://github.com/21centuryweather/hk25-AusCyclones)
* [Model intercomparison for extremes precipitation](https://github.com/21centuryweather/hk25-AusNode-ExtremePrecipitation)
* [Unravelling the representation of Tropical Convergence Zones in km-scale model runs](https://github.com/21centuryweather/hk25-AusNode-TConvZones)
* [The relationship of cloud size and number with large-scale environment for precipitation in high-resolution models](https://github.com/21centuryweather/hk25-AusNode-LargeScaleP)
* [Diurnal cycle of coastal winds and rainfall](https://github.com/21centuryweather/hk25-AusNode-coastal)
* [Precipitation/soil moisture feedback: positive or negative?](https://github.com/21centuryweather/hk25-AusNode-land)
* [The hunt for city-driven atmospheric circulation](https://github.com/21centuryweather/hk25-CityCirc)
* [Convectively-Coupled Systems in the Tropics as Simulated in Global Storm Resolving Models](https://github.com/21centuryweather/hk25-AusNode-ConvTrop)






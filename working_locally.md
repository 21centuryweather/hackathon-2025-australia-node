# Working on your laptop (not on Gadi)

If you want or need to work locally instead of in Gadi, you will need to setup a conda environment and relay on online data. We recommend you to develop the code using a low resolution version of the data (zoom 4 or 5) as bandwidth and RAM will be limited. 

## Conda environment

Use the [`environment.yaml`](https://github.com/digital-earths-global-hackathon/tools/blob/main/python_envs/environment.yaml) provided by the Digital Earths Global Hackathon team to build the environment. This includes the necessary libraries to work with zarr and the healpix grid. 

0. Do you have conda installed?
1. Download the yaml file into your computer
2. Run:

```python
conda env create --name NAME --file path/to/environment.yaml
```
3. Activate your new environment with

```python
conda activate NAME
```


## Online data

A few nodes have put some of the data available online, including some of the simulations, observations and reanalysis. The best way to get the list of available data is by checking the [intake catalog](https://digital-earths-global-hackathon.github.io/catalog/) for the hackathon.

```
import intake
cat = intake.open_catalog("https://digital-earths-global-hackathon.github.io/catalog/catalog.yaml")["online"]
list(cat)
```

[Here is a nice example on how to work with the catalog and online data](https://github.com/digital-earths-global-hackathon/hk25-teams/blob/main/hk25-tutorials/simple_plot.ipynb).

You can also check the list along with the URLs [in this yaml file](https://github.com/digital-earths-global-hackathon/catalog/blob/main/online/main.yaml).

> [!NOTE]
> If you read any data and you get a bunch of `nan`s it means that the data is not available yet. 
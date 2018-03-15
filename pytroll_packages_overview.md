# PyTroll package summary overview, dependencies, level of maturity and usage

Below is a short overview of all packages developed by and/or maintained by the PyTroll community. Included is their level of maturity, mutual interdependencies, and known operational usage (as of March 2018).

There is a great spread in the size and complexity of the packages, and they may address rather different issues related to the processing and handling of satellite data.

If you are new to PyTroll, and have some satellite data you want to read and display, you should start out by getting familiar with SatPy!

## All general PyTroll packages

### SatPy

* **Summary**: Python package for earth-observing satellite data processing. Reading many level-1 and -2 products, resamples the data, generates composite RGB imagery, and saves in a few standard formats such as netCDF, geoTIFF or png. Satpy is replacing Mpop (see below).

* **Development intensity**: High

* **Maturity**: Becoming mature

* **PyTroll dependencies**: PyResample, PyKdtree, Trollimage, Trollsift

* **Optional PyTroll dependencies**: PySpectral, PyOrbital, PyGAC, Mipp, Python-geotiepoints, Pytroll-schedule.

* **Other dependencies**: NumPy, Pillow, Pyyaml, Six

* **In 24/7 production @**: FMI, MeteoSwiss, DWD, ESTEA, LEGMC, IMO, ECCC...

### Trollimage:

* **Summary**: Imaging package for pytroll

* **Development intensity**: Medium

* **Maturity**: Mature

* **PyTroll dependencies**: None

* **Optional PyTroll dependencies**: None

* **Other dependencies**: NumPy, Pillow, Six

* **24/7 production @**: FMI, SMHI, MeteoSwiss, ESTEA, LEGMC, IMO, ECCC, ...

### PyOrbital:

* **Summary**: Orbital and astronomy computations in python

* **Development intensity**: Low

* **Maturity**: Mature

* **PyTroll dependencies**: None

* **Optional PyTroll dependencies**: None

* **Other dependencies**: NumPy

* **24/7 production @**: FMI, SMHI, DMI, ESTEA, LEGMC, IMO, ECCC, ...

### PyResample:

* **Summary**: Geospatial image resampling in Python

* **Development intensity**: Medium

* **Maturity**: Mature

* **PyTroll dependencies**: PyKDTree

* **Optional PyTroll dependencies**: None

* **Other dependencies**: Pyproj, NumPy, Pyyaml, Six, confiobj, setuptools, Numexpr (optional), Dask (optional), Matplotlib (optional), Basemap (optional), Pillow (optional)

* **24/7 production @**: FMI, SMHI, DMI, Met Norway, MeteoSwiss, DWD, CNMCA, ESTEA, LEGMC, IMO, ECCC, ...

### PyKDTree

* **Summary**: Fast kd-tree implementation in Python

* **Development intensity**: Low

* **Maturity**: Mature

* **PyTroll dependencies**: None

* **Optional PyTroll dependencies**: None

* **Other dependencies**: NumPy, OpenMP

* **24/7 production @**: FMI, DMI, SMHI, Met Norway, MeteoSwiss, DWD, CNMCA, ESTEA, LEGMC,  IMO, ECCC,.

### Python-geotiepoints

* **Summary**: Interpolation and extrapolation of geographic (lon, lat) tie points

* **Development intensity**: Medium

* **Maturity**: Mature

* **PyTroll dependencies**: None

* **Optional PyTroll dependencies**: None

* **Other dependencies**: NumPy, Scipy, Pandas, Cython (optional)

* **24/7 production @**: DMI, FMI, ESTEA, SMHI, LEGMC, IMO, ECCC

### PySpectral

* **Summary**: Read and manipulate satellite sensor spectral responses and solar irradiance spectra

* **Development intensity**: Medium

* **Maturity**: Mature

* **PyTroll dependencies**: None

* **Optional PyTroll dependencies**: None

* **Other dependencies**: NumPy, Scipy, h5py, Pyyaml, tqdm, requests, appdirs, Six, xlrd (optional), Matplotlib (optional)

* **24/7 production @**: FMI, SMHI, IMO, ECCC


## Institutes/entities

* CNMCA: Centro Nazionale di Meteorologia e Climatologia Aeronautica (National Center for Aeronautical Meteorology and Climatology, Italy)

* DMI: Danish Meteorological Institute

* DWD: Deutscher Wetter Dienst (German weather service)

* ECCC: Environment and Climate Change Canada

* ESTEA: Estonian Environment Agency

* FMI: Finnish Meteorological Institute

* IMO: Icelandic Meteorological Office

* LEGMC: Latvian Environment, Geology and Meteorology Centre

* Met Norway: Norwegian Meteorological Institute

* MeteoSwiss: Swiss Federal Office for Meteorology and Climatology

* SMHI: Swedish Meteorological and Hydrological Institute

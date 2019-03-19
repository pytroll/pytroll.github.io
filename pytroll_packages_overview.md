# PyTroll package summary overview, dependencies, level of maturity and usage

Below is a short overview of all packages developed by and/or maintained by the PyTroll community. Included is their
level of maturity, mutual interdependencies, and known operational usage (as of March 2018).

There is a great spread in the size and complexity of the packages, and they may address rather different issues
related to the processing and handling of satellite data.

If you are new to PyTroll, and have some satellite data you want to read and display, you should start out by getting
familiar with SatPy!

## All general PyTroll packages

All packages are python 2.7 and 3.4+ compatible unless specified otherwise. See the individual package documentation
for details or limitations. Due to the deprecation of Python 2, support in Pytroll packages is not guaranteed
after 2019. If a package below does not work on a certain version of python please file a bug in the appropriate github
repository.

### SatPy

* **Summary**: Python package for earth-observing satellite data processing. Reading many level-1 and -2 products,
               resamples the data, generates composite RGB imagery, and saves in a few standard formats such as netCDF,
               geoTIFF or png. Satpy is replacing Mpop (see below).

* **Development intensity**: High

* **Maturity**: Becoming mature

* **PyTroll dependencies**: PyResample, PyKdtree, Trollimage, Trollsift

* **Optional PyTroll dependencies**: PySpectral, PyOrbital, PyGAC, Mipp, Python-geotiepoints, Pytroll-schedule.

* **Other dependencies**: NumPy, Pillow, Pyyaml, Six

* **In 24/7 production @**: FMI, MeteoSwiss, DWD, ESTEA, LEGMC, IMO, ECCC, Met Norway,...

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

* **24/7 production @**: FMI, SMHI, DMI, ESTEA, LEGMC, IMO, ECCC, Met Norway, ...

### PyResample:

* **Summary**: Geospatial image resampling in Python

* **Development intensity**: Medium

* **Maturity**: Mature

* **PyTroll dependencies**: PyKDTree

* **Optional PyTroll dependencies**: None

* **Other dependencies**: Pyproj, NumPy, Pyyaml, Six, confiobj, setuptools, Numexpr (optional), Dask (optional), Matplotlib (optional), Basemap (optional), Pillow (optional)

* **24/7 production @**: FMI, SMHI, DMI, Met Norway, MeteoSwiss, DWD, COMet, ESTEA, LEGMC, IMO, ECCC, ...

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


### Posttroll

* **Summary**: High-level messaging system for pytroll

* **Development intensity**: Medium

* **Maturity**: Mature

* **PyTroll dependencies**: None

* **Optional PyTroll dependencies**: None

* **Other dependencies**: Pyzmq

* **24/7 production @**: FMI, DWD, SMHI, Met Norway

### Trollcast

* **Summary**: Polar weather satellite data exchange tool

* **Development intensity**: Low

* **Maturity**: Mature

* **PyTroll dependencies**: Pyorbital, Posttroll, Trollsift

* **Optional PyTroll dependencies**: None

* **Other dependencies**: Pyzmq, NumPy, Pyinotify

* **24/7 production @**: FMI, LEGMC, SMHI, IMO, Met Norway, ...

### Pytroll-schedule

* **Summary**: Reception scheduling of polar weather satellites

* **Development intensity**: Low

* **Maturity**: Mature

* **PyTroll dependencies**: PyOrbital, PyResample

* **Optional PyTroll dependencies**:

* **Other dependencies**: NumPy, Basemap (optional)

* **24/7 production @**: FMI, SMHI, DWD, IMO, Met Norway, ...

### Trollsift

* **Summary**: Formatting, parsing and filtering satellite granule file names

* **Development intensity**: Low

* **Maturity**: Mature

* **PyTroll dependencies**: None

* **Optional PyTroll dependencies**: None

* **Other dependencies**: Six

* **24/7 production @**: FMI, DWD, SMHI, IMO, Met Norway, ...

### PyCoast

* **Summary**: Python package to add coastlines, borders and rivers to raster images using data from the GSHHS and WDBII datasets
* **Development intensity**: Low

* **Maturity**: Mature

* **PyTroll dependencies**: None

* **Optional PyTroll dependencies**: None

* **Other dependencies**: Pyshp, NumPy, Pyproj, Pillow, Six

* **24/7 production @**: MeteoSwiss, FMI, SMHI, ESTEA, LEGMC, IMO, ECCC, Met Norway, COMet, ...

### PyDecorate

* **Summary**: Package for decorating PIL/Pillow images with logos, texts, and color scales.

* **Development intensity**: Low

* **Maturity**: Mature

* **PyTroll dependencies**: None

* **Optional PyTroll dependencies**: None

* **Other dependencies**: Pillow

* **24/7 production @**: IMO, ECCC, MeteoSwiss, COMet, ...

### Trollbufr

* **Summary**: A light weight pure Python BUFR reader, and writer

* **Development intensity**: Medium

* **Maturity**: Medium

* **PyTroll dependencies**: None

* **Optional PyTroll dependencies**: None

* **Other dependencies**: None

* **24/7 production @**: 

### Pytroll-collectors

* **Summary**: Collector modules for Pytroll

* **Development intensity**: Low

* **Maturity**: Mature

* **PyTroll dependencies**: PyKDTree, Mpop, Posttroll, Trollsift, pytroll-schedule, PyResample, PyCoast

* **Optional PyTroll dependencies**:

* **Other dependencies**: Pyinotify, netifaces, Pillow

* **24/7 production @**: FMI, SMHI, Met Norway, ...

### Trollduction
* **Summary**: Framework for operational weather satellite image batch production.

* **Development intensity**: Frozen. Being replaced by Trollflow

* **Maturity**: Mature

* **PyTroll dependencies**: Mpop, Posttroll, PyResample, PyKDTree, Trollimage, PyOrbital, Trollsift, Pytroll-schedule, Pytroll-collectors

* **Optional PyTroll dependencies**: None

* **Other dependencies**: Netifaces, netCDF4

* **24/7 production @**: DWD, SMHI

### Trollflow

* **Summary**: A small Python workflow execution framework

* **Development intensity**: Medium

* **Maturity**: Becoming mature

* **PyTroll dependencies**: None

* **Optional PyTroll dependencies**: None

* **Other dependencies**: Pyyaml, Mock

* **24/7 production @**: FMI, DWD

### Trollflow-sat

* **Summary**: Trollflow plug-ins for satellite data processing

* **Development intensity**: Medium

* **Maturity**: Becoming mature

* **PyTroll dependencies**: SatPy or mpop, PyResample, Posttroll, Trollsift

* **Optional PyTroll dependencies**: PyOrbital

* **Other dependencies**: Pyyaml

* **24/7 production @**: FMI, DWD


### PyGAC

* **Summary**: A python package to read and calibrate NOAA AVHRR GAC data

* **Development intensity**: Low

* **Maturity**: Mature

* **PyTroll dependencies**: PyOrbital

* **Optional PyTroll dependencies**: None

* **Other dependencies**: NumPy, h5py, docutils

* **24/7 production @**: 

### Pyninjotiff

* **Summary**: Python library for writing Ninjo-compatible TIFF files

* **Development intensity**: Low

* **Maturity**: Mature

* **PyTroll dependencies**: None

* **Optional PyTroll dependencies**: None

* **Other dependencies**: NumPy, Six

* **24/7 production @**: MeteoSwiss

### Pytroll-db

* **Summary**: Database interface for pytroll

* **Development intensity**: Very low

* **Maturity**: Mature

* **PyTroll dependencies**: PyOrbital, Posttroll

* **Optional PyTroll dependencies**: None

* **Other dependencies**: Geoalchemy2, Sqlalchemy, Shapely, Psycop2, Paramiko

* **24/7 production @**:

### Aggdraw

* **Summary**: Clone of the aggdraw module

* **Development intensity**: Low

* **Maturity**: Mature

* **PyTroll dependencies**: None

* **Optional PyTroll dependencies**: None

* **Other dependencies**: None

* **24/7 production @**: MeteoSwiss, FMI, LEGMC, SMHI, ECCC, Met Norway, ...

### Mpop

* **Summary**: Being replaced by SatPy

* **Development intensity**: Low. Frozen: No new features are being implemented, only bug-fixes.

* **Maturity**: Mature

* **PyTroll dependencies**: PyResample

* **Optional PyTroll dependencies**: Mipp, PySpectral, PyOrbital, PyGAC

* **Other dependencies**: NumPy, Pillow

* **In 24/7 production @**: FMI, SMHI, DMI, Met Norway, MeteoSwiss, DWD, COMet, ESTEA, LEGMC, IMO... 

### Mipp

* **Summary**: Lower level library providing mainly level-1 readers for mpop (SatPy). Originally first of all for HRIT/XRIT data formats (geostationary satellites) but also supports some SAR data formats. 

* **Development intensity**: Low. Most readers are now implemented in SatPy.

* **Maturity**: Mature

* **PyTroll dependencies**: None

* **Optional PyTroll dependencies**: None

* **Other dependencies**: NumPy

* **In 24/7 production @**: FMI, DMI, SMHI, Met Norway, MeteoSwiss, DWD, COMet, LEGMC, IMO, ESTEA...


## Pytroll runners

Below we list various Pytroll runners for specific tasks and applications. Many of these are still a bit specific to SMHI. When it becomes relevant the aim is to make those more general and thus useful to more entities. They are included here, so new users are invited to take off using those existing runners and make them more general to also serve their needs.

### Pytroll-cspp-runner

* **Summary**: PyTroll runner for the SNPP/JPSS pre-processing (RDR to SDR) with the CSPP package

* **Development intensity**: Low

* **Maturity**: Not yet general enough.

* **PyTroll dependencies**: Posttroll

* **Optional PyTroll dependencies**: None

* **Other dependencies**: None

* **24/7 production @**: SMHI

### Pytroll-aapp-runner

* **Summary**: PyTroll runner for NOAA/Metop pre-processing with the NWPSAF/AAPP package

* **Development intensity**: Low

* **Maturity**: Getting mature

* **PyTroll dependencies**: Posttroll

* **Optional PyTroll dependencies**: None

* **Other dependencies**: None

* **24/7 production @**: FMI, SMHI, Met Norway

### Pytroll-pps-runner

* **Summary**: PyTroll runner for the NWCSAF/PPS cloud processing package

* **Development intensity**: Low

* **Maturity**: Not yet general enough. 

* **PyTroll dependencies**: Posttroll

* **Optional PyTroll dependencies**: None

* **Other dependencies**: None

* **24/7 production @**: FMI (with local modifications), SMHI, Met Norway

### Pytroll-osisaf-runner

* **Summary**: Pytroll runner for OSISAF SST products

* **Development intensity**: Low

* **Maturity**: Not general enough. Specific to SMHI

* **PyTroll dependencies**: Posttroll, Mpop

* **Optional PyTroll dependencies:** None

* **Other dependencies**: None

* **24/7 production @**: SMHI

### Pytroll-modis-runner

* **Summary**: PyTroll runner for MODIS pre-processing (PDS to level-1) with SeaDAS

* **Development intensity**: Low

* **Maturity**: Not general enough. Specific to SMHI

* **PyTroll dependencies**: Posttroll

* **Optional PyTroll dependencies**: None

* **Other dependencies**: None

* **24/7 production @**: SMHI, Met Norway


## Institutes/entities

* COMet: Centro Operativo per la Meteorologia (Operative Center for Meteorology, Italy)

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

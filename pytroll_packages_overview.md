# Pytroll package summary overview, dependencies, level of maturity and usage

Below is a short overview of all packages developed by and/or maintained by the Pytroll community. Included is their
level of maturity, mutual interdependencies, and known operational usage (as of March 2018).

There is a great spread in the size and complexity of the packages, and they may address rather different issues
related to the processing and handling of satellite data.

If you are new to Pytroll, and have some satellite data you want to read and display, you should start out by getting
familiar with Satpy!

## All general Pytroll packages

All packages require Python 3 (Python 2 is no longer supported).
The specific version required varies per package but usually packages support at
least the versions of Python released in the last 2--3 years.  See the
individual package documentation for details or limitations.

### Satpy

* **Summary**: Python package for earth-observing satellite data processing. Reading many level-1 and -2 products,
               resamples the data, generates composite RGB imagery, and saves in a few standard formats such as netCDF,
               geoTIFF or png. Satpy is replacing Mpop (see below).

* **Development intensity**: High

* **Maturity**: Becoming mature

* **GitHub**: <https://github.com/pytroll/satpy>

* **Docs**: <https://satpy.readthedocs.io>

* **Pytroll dependencies**: Pyresample, Pykdtree, Trollimage, Trollsift

* **Optional Pytroll dependencies**: Pyspectral, Pyorbital, PyGAC, Python-geotiepoints, Pytroll-schedule.

* **Other dependencies**: NumPy, Pillow, Pyyaml, Six

* **In 24/7 production @**: FMI, MeteoSwiss, DWD, ESTEA, LEGMC, IMO, ECCC, Met Norway,...

### Trollimage:

* **Summary**: Imaging package for Pytroll

* **Development intensity**: Medium

* **GitHub**: <https://github.com/pytroll/trollimage>

* **Docs**: <https://trollimage.readthedocs.io>

* **Maturity**: Mature

* **Pytroll dependencies**: None

* **Optional Pytroll dependencies**: None

* **Other dependencies**: NumPy, Pillow, Six

* **24/7 production @**: FMI, SMHI, MeteoSwiss, ESTEA, LEGMC, IMO, ECCC, ...

### Pyorbital:

* **Summary**: Orbital and astronomy computations in python

* **Development intensity**: Low

* **GitHub**: <https://github.com/pytroll/pyorbital>

* **Docs**: <https://pyorbital.readthedocs.io>

* **Maturity**: Mature

* **Pytroll dependencies**: None

* **Optional Pytroll dependencies**: None

* **Other dependencies**: NumPy

* **24/7 production @**: FMI, SMHI, DMI, ESTEA, LEGMC, IMO, ECCC, Met Norway, ...

### Pyresample:

* **Summary**: Geospatial image resampling in Python

* **Development intensity**: Medium

* **GitHub**: <https://github.com/pytroll/pyresample>

* **Docs**: <https://pyresample.readthedocs.io>

* **Maturity**: Mature

* **Pytroll dependencies**: PyKDTree

* **Optional Pytroll dependencies**: None

* **Other dependencies**: Pyproj, NumPy, Pyyaml, Six, confiobj, setuptools, Numexpr (optional), Dask (optional), Matplotlib (optional), Basemap (optional), Pillow (optional)

* **24/7 production @**: FMI, SMHI, DMI, Met Norway, MeteoSwiss, DWD, COMet, ESTEA, LEGMC, IMO, ECCC, ...

### PyKDTree

* **Summary**: Fast kd-tree implementation in Python

* **Development intensity**: Low

* **GitHub**: <https://github.com/pytroll/pykdtree>

* **Docs**: 

* **Maturity**: Mature

* **Pytroll dependencies**: None

* **Optional Pytroll dependencies**: None

* **Other dependencies**: NumPy, OpenMP

* **24/7 production @**: FMI, DMI, SMHI, Met Norway, MeteoSwiss, DWD, CNMCA, ESTEA, LEGMC,  IMO, ECCC,.

### Python-geotiepoints

* **Summary**: Interpolation and extrapolation of geographic (lon, lat) tie points

* **Development intensity**: Medium

* **GitHub**: <https://github.com/pytroll/python-geotiepoints>

* **Docs**: <https://python-geotiepoints.readthedocs.io/en/latest/>

* **Maturity**: Mature

* **Pytroll dependencies**: None

* **Optional Pytroll dependencies**: None

* **Other dependencies**: NumPy, Scipy, Pandas, Cython (optional)

* **24/7 production @**: DMI, FMI, ESTEA, SMHI, LEGMC, IMO, ECCC

### Pyspectral

* **Summary**: Read and manipulate satellite sensor spectral responses and solar irradiance spectra

* **Development intensity**: Medium

* **GitHub**: <https://github.com/pytroll/pyspectral>

* **Docs**: <https://pyspectral.readthedocs.io>

* **Maturity**: Mature

* **Pytroll dependencies**: None

* **Optional Pytroll dependencies**: None

* **Other dependencies**: NumPy, Scipy, h5py, Pyyaml, tqdm, requests, appdirs, Six, xlrd (optional), Matplotlib (optional)

* **24/7 production @**: FMI, SMHI, IMO, ECCC


### Posttroll

* **Summary**: High-level messaging system for Pytroll

* **Development intensity**: Medium

* **GitHub**: <https://github.com/pytroll/posttroll>

* **Docs**: <https://posttroll.readthedocs.io>

* **Maturity**: Mature

* **Pytroll dependencies**: None

* **Optional Pytroll dependencies**: None

* **Other dependencies**: Pyzmq

* **24/7 production @**: FMI, DWD, SMHI, Met Norway

### Trollcast

* **Summary**: Polar weather satellite data exchange tool

* **Development intensity**: Low

* **GitHub**: <https://github.com/pytroll/trollcast>

* **Docs**: <https://trollcast.readthedocs.io>

* **Maturity**: Mature

* **Pytroll dependencies**: Pyorbital, Posttroll, Trollsift

* **Optional Pytroll dependencies**: None

* **Other dependencies**: Pyzmq, NumPy, Pyinotify

* **24/7 production @**: FMI, LEGMC, SMHI, IMO, Met Norway, ...

### Pytroll-schedule

* **Summary**: Reception scheduling of polar weather satellites

* **Development intensity**: Low

* **GitHub**: <https://github.com/pytroll/pytroll-schedule>

* **Docs**: <https://pytroll-schedule.readthedocs.io>

* **Maturity**: Mature

* **Pytroll dependencies**: Pyorbital, Pyresample

* **Optional Pytroll dependencies**:

* **Other dependencies**: NumPy, Basemap (optional)

* **24/7 production @**: FMI, SMHI, DWD, IMO, Met Norway, ...

### Trollsift

* **Summary**: Formatting, parsing and filtering satellite granule file names

* **Development intensity**: Low

* **GitHub**: <https://github.com/pytroll/trollsift>

* **Docs**: <https://trollsift.readthedocs.io>

* **Maturity**: Mature

* **Pytroll dependencies**: None

* **Optional Pytroll dependencies**: None

* **Other dependencies**: Six

* **24/7 production @**: FMI, DWD, SMHI, IMO, Met Norway, ...

### Pycoast

* **Summary**: Python package to add coastlines, borders and rivers to raster images using data from the GSHHS and WDBII datasets
* **Development intensity**: Low

* **Maturity**: Mature

* **GitHub**: <https://github.com/pytroll/pycoast>

* **Docs**: <https://pycoast.readthedocs.io>

* **Pytroll dependencies**: None

* **Optional Pytroll dependencies**: None

* **Other dependencies**: Pyshp, NumPy, Pyproj, Pillow, Six

* **24/7 production @**: MeteoSwiss, FMI, SMHI, ESTEA, LEGMC, IMO, ECCC, Met Norway, COMet, ...

### Pydecorate

* **Summary**: Package for decorating PIL/Pillow images with logos, texts, and color scales.

* **Development intensity**: Low

* **Maturity**: Mature

* **GitHub**: <https://github.com/pytroll/pydecorate>

* **Docs**: <https://pydecorate.readthedocs.io>

* **Pytroll dependencies**: None

* **Optional Pytroll dependencies**: None

* **Other dependencies**: Pillow

* **24/7 production @**: IMO, ECCC, MeteoSwiss, COMet, ...

### Trollbufr

* **Summary**: A light weight pure Python BUFR reader, and writer

* **Development intensity**: Medium

* **Maturity**: Medium

* **GitHub**: <https://github.com/pytroll/trollbufr>

* **Docs**: <https://trollbufr.readthedocs.io>

* **Pytroll dependencies**: None

* **Optional Pytroll dependencies**: None

* **Other dependencies**: None

* **24/7 production @**: 

### Pytroll-collectors

* **Summary**: Collector modules for Pytroll

* **Development intensity**: Low

* **Maturity**: Mature

* **GitHub**: <https://github.com/pytroll/pytroll-collectors>

* **Docs**: 

* **Pytroll dependencies**: PyKDTree, Mpop, Posttroll, Trollsift, pytroll-schedule, Pyresample, Pycoast

* **Optional Pytroll dependencies**:

* **Other dependencies**: Pyinotify, netifaces, Pillow

* **24/7 production @**: FMI, SMHI, Met Norway, ...

### Trollflow2

* **Summary**: A small Python workflow execution framework

* **Development intensity**: Medium

* **Maturity**: Becoming mature

* **GitHub**: <https://github.com/pytroll/trollflow2>

* **Docs**: 

* **Pytroll dependencies**: None

* **Optional Pytroll dependencies**: None

* **Other dependencies**: Pyyaml, Mock

* **24/7 production @**: FMI, DWD

### PyGAC

* **Summary**: A python package to read and calibrate NOAA AVHRR GAC data

* **Development intensity**: Low

* **Maturity**: Mature

* **GitHub**: <https://github.com/pytroll/pygac>

* **Docs**: <https://pygac.readthedocs.io>

* **Pytroll dependencies**: Pyorbital

* **Optional Pytroll dependencies**: None

* **Other dependencies**: NumPy, h5py, docutils

* **24/7 production @**: 

### Pyninjotiff

* **Summary**: Python library for writing Ninjo-compatible TIFF files

* **Development intensity**: Low

* **Maturity**: Mature

* **GitHub**: <https://github.com/pytroll/pyninjotiff>

* **Docs**: 

* **Pytroll dependencies**: None

* **Optional Pytroll dependencies**: None

* **Other dependencies**: NumPy, Six

* **24/7 production @**: MeteoSwiss, DWD

### Pytroll-db

* **Summary**: Database interface for pytroll

* **Development intensity**: Very low

* **Maturity**: Mature

* **GitHub**: <https://github.com/pytroll/pytroll-db>

* **Docs**: 

* **Pytroll dependencies**: Pyorbital, Posttroll

* **Optional Pytroll dependencies**: None

* **Other dependencies**: Geoalchemy2, Sqlalchemy, Shapely, Psycop2, Paramiko

* **24/7 production @**:

### Aggdraw

* **Summary**: Clone of the aggdraw module

* **Development intensity**: Low

* **Maturity**: Mature

* **GitHub**: <https://github.com/pytroll/aggdraw>

* **Docs**: <https://aggdraw.readthedocs.io>

* **Pytroll dependencies**: None

* **Optional Pytroll dependencies**: None

* **Other dependencies**: None

* **24/7 production @**: MeteoSwiss, FMI, LEGMC, SMHI, ECCC, Met Norway, ...

### Fogpy

* **Summary**: Retrieve fog from SEVIRI or ABI

* **Development intensity**: Low

* **Maturity**: experimental

* **GitHub**: <https://github.com/pytroll/fogpy>

* **Docs**: <https://fogpy.readthedocs.io>

* **Pytroll dependencies**: Satpy

* **24/7 production @**: N/A

## Pytroll runners

Below we list various Pytroll runners for specific tasks and applications. Many of these are still a bit specific to SMHI. When it becomes relevant the aim is to make those more general and thus useful to more entities. They are included here, so new users are invited to take off using those existing runners and make them more general to also serve their needs.

### Pytroll-cspp-runner

* **Summary**: Pytroll runner for the SNPP/JPSS pre-processing (RDR to SDR) with the CSPP package

* **Development intensity**: Low

* **Maturity**: Not yet general enough.

* **GitHub**: <https://github.com/pytroll/pytroll-cspp-runner>

* **Docs**: 

* **Pytroll dependencies**: Posttroll

* **Optional Pytroll dependencies**: None

* **Other dependencies**: None

* **24/7 production @**: SMHI

### Pytroll-aapp-runner

* **Summary**: Pytroll runner for NOAA/Metop pre-processing with the NWPSAF/AAPP package

* **Development intensity**: Low

* **Maturity**: Getting mature

* **GitHub**: <https://github.com/pytroll/pytroll-aapp-runner>

* **Docs**: 

* **Pytroll dependencies**: Posttroll

* **Optional Pytroll dependencies**: None

* **Other dependencies**: None

* **24/7 production @**: FMI, SMHI, Met Norway

### Pytroll-pps-runner

* **Summary**: Pytroll runner for the NWCSAF/PPS cloud processing package

* **Development intensity**: Low

* **Maturity**: Not yet general enough. 

* **GitHub**: <https://github.com/pytroll/pytroll-pps-runner>

* **Docs**: 

* **Pytroll dependencies**: Posttroll

* **Optional Pytroll dependencies**: None

* **Other dependencies**: None

* **24/7 production @**: FMI (with local modifications), SMHI, Met Norway

### Pytroll-osisaf-runner

* **Summary**: Pytroll runner for OSISAF SST products

* **Development intensity**: Low

* **Maturity**: Not general enough. Specific to SMHI

* **GitHub**: <https://github.com/pytroll/pytroll-osisaf-runner>

* **Docs**: 

* **Pytroll dependencies**: Posttroll, Mpop

* **Optional Pytroll dependencies:** None

* **Other dependencies**: None

* **24/7 production @**: SMHI

### Pytroll-modis-runner

* **Summary**: Pytroll runner for MODIS pre-processing (PDS to level-1) with SeaDAS

* **Development intensity**: Low

* **Maturity**: Not general enough. Specific to SMHI

* **GitHub**: <https://github.com/pytroll/pytroll-modis-runner>

* **Docs**: 

* **Pytroll dependencies**: Posttroll

* **Optional Pytroll dependencies**: None

* **Other dependencies**: None

* **24/7 production @**: SMHI, Met Norway

## Obsolete, historical, retired, and archived packages

Those packages have served their purpose, but are no longer being actively
developed.  Their use is not recommended.  If you are still using them,
we recommend upgrading to the current replacement.

### Mpop

* **Replacement**: Satpy

* **GitHub**: <https://github.com/pytroll/mpop>

* **Docs**: <https://mpop.readthedocs.io>

* **Pytroll dependencies**: Pyresample

* **Optional Pytroll dependencies**: Pyspectral, Pyorbital, PyGAC

* **Other dependencies**: NumPy, Pillow

* **In 24/7 production @**: FMI, SMHI, DMI, Met Norway, MeteoSwiss, DWD, COMet, ESTEA, LEGMC, IMO... 

### Mipp

* **Replacement**: Satpy

* **Summary**: Lower level library providing mainly level-1 readers for mpop (Satpy). Originally first of all for HRIT/XRIT data formats (geostationary satellites) but also supports some SAR data formats. 

* **GitHub**: <https://github.com/pytroll/mipp>

* **Docs**: <https://mipp.readthedocs.io>

* **Pytroll dependencies**: None

* **Optional Pytroll dependencies**: None

* **Other dependencies**: NumPy

* **In 24/7 production @**: FMI, DMI, SMHI, Met Norway, MeteoSwiss, DWD, COMet, LEGMC, IMO, ESTEA...

### Trollduction

* **Replacement**: Trollflow2

* **Summary**: Framework for operational weather satellite image batch production.

* **GitHub**: <https://github.com/pytroll/trollduction>

* **Docs**: <https://trollduction.readthedocs.io>

* **Pytroll dependencies**: Mpop, Posttroll, Pyresample, PyKDTree, Trollimage, Pyorbital, Trollsift, Pytroll-schedule, Pytroll-collectors

* **Optional Pytroll dependencies**: None

* **Other dependencies**: Netifaces, netCDF4

* **24/7 production @**: DWD, SMHI

### Trollflow

* **Replacement**: Trollflow2

* **GitHub**: <https://github.com/pytroll/trollflow>

* **Docs**: 

* **Pytroll dependencies**: None

* **Optional Pytroll dependencies**: None

* **Other dependencies**: Pyyaml, Mock

* **24/7 production @**: FMI, DWD

### Trollflow-sat

* **Replacement**: Trollflow2

* **Summary**: Trollflow plug-ins for satellite data processing

* **GitHub**: <https://github.com/pytroll/trollflow-sat>

* **Docs**: 

* **Pytroll dependencies**: Satpy or mpop, Pyresample, Posttroll, Trollsift

* **Optional Pytroll dependencies**: Pyorbital

* **Other dependencies**: Pyyaml

* **24/7 production @**: FMI, DWD


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

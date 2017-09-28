> Suomi-NPP, NPP, JPSS, SDR, AAPP, CSPP, HRPT, TerraSAR-X, COSMO-SkyMed, Radarsat-2, Himawari, Sentinel, SLSTR, OLCI, Sentinel-1, Sentinel-2, Sentinel-3, GOES-R, ABI, GOES-16, read, reading, reader, process, processing, python, pytroll, weather, satellite, data

## Pytroll?

The objective of Pytroll is to provide an easy to use, modular, free and open source python framework for the processing of earth observation satellite data. The provided python packages are designed to be used both in R&D environments and in 24/7 operational production.

The focus is on atmospheric applications and imaging sensors, but as seen from the list of supported satellite sensors below the data that can be handled py Pytroll allows the usage in a wide range of earth sciences.

For a quick and easy overview of what Pytroll can possibly offer for you have a look at the [Pytroll tutorial](https://docs.google.com/presentation/d/1-ast62mC7X0z7504gSJCthRnQP-8LrU0Pz_CNxUx0Ag/edit#slide=id.p) which was shown at the 2016 Eumetsat conference in Darmstadt Wednesday September 28

If you want to contact us, you can use the following mailing list: <https://groups.google.com/group/pytroll> or chat with us on the pytroll slack: <https://pytrollslackin.herokuapp.com/> or on the pytroll IRC channel on freenode: <irc://irc.freenode.net/pytroll>

> **note**
>
> Centre Météorologie Spatiale, Météo-France, Lannion, September 2017
>
> <table>
> <col width="19%" />
> <tbody>
> <tr class="odd">
> <td align="left"><blockquote>
> <p><embed src="_static/PytrollGroupLannion20170914_small.JPG%0A%20:width:%20770px" /></p>
> </blockquote></td>
> </tr>
> <tr class="even">
> <td align="left"></td>
> </tr>
> </tbody>
> </table>
>
The available pytroll python packages at the moment are:

-   [pyresample](http://github.com/pytroll/pyresample) for resampling satellite data
-   [mpop](http://github.com/pytroll/mpop) for reading and processing weather satellite data
-   [satpy](https://github.com/pytroll/satpy) A refactored [mpop](http://github.com/pytroll/mpop) (for reading and processing weather satellite data)
-   [mipp](http://github.com/pytroll/mipp) for reading (mostly HRIT/LRIT formated) weather satellite data
-   [pycoast](http://github.com/pytroll/pycoast) for putting coastlines, borders and rivers on an image
-   [pyorbital](http://github.com/pytroll/pyorbital) for computing satellite orbital parameters and reading TLE's
-   [posttroll](http://github.com/pytroll/posttroll) a higher-level messaging library for pytroll
-   [pykdtree](https://github.com/storpipfugl/pykdtree) for really fast nearest neighbour search
-   [pythonggeotiepoints](http://github.com/pytroll/python-geotiepoints) for interpolating (and extrapolation) geographic tiepoints
-   [trollimage](https://github.com/pytroll/trollimage) the new image packagse for pytroll (replaces and enhances the image.py module in mpop)
-   [trollsift](https://github.com/pytroll/trollsift) for the formatting, parsing and filtering of satellite granule file names
-   [pyspectral](https://github.com/pytroll/pyspectral) to read and manipulate satellite sensor spectral responses and solar irradiance spectra
-   [pydecorate](http://code.google.com/p/pydecorate) to simplify the drawing of logos, text labels, color scales and legends onto images
-   [trollduction](https://github.com/pytroll/trollduction) a framework for satellite batch processing
-   [pytrollsschedule](https://github.com/pytroll/pytroll-schedule) to generate optimized satellite schedules for polar reception stations
-   [trollcast](http://github.com/pytroll/trollcast) for realtime sharing of weather satellite data
-   [pygac](https://github.com/pytroll/pygac) to read NOAA AVHRR Global Area Coverage (GAC) data and apply state of the art calibration and navigation

Some more packages are in the process of being developed (you're very welcome to have a look and give us a hand):

-   [pygranules](http://pygranule.readthedocs.org/en/latest) for validating, fetching and scheduling satellite data granules
-   [trollbufr](https://github.com/alexmaul/trollbufr) for reading BUFR files

Satellites supported (imager instruments) at the moment by the reader/processor modules include:

> -   Meteosat series (tested with 7, 8, 9, 10, 11)
> -   GOES series, in HRIT/LRIT format (tested with 11, 12, 13, 15, 16)
> -   MTSAT series, in HRIT/LRIT format (tested with 1R, 2)
> -   Himawari 8 & 9, in HRIT/LRIT format
> -   Himawari 8 & 9, standard format ([satpy](https://github.com/pytroll/satpy) only)
> -   Electro L, in HRIT/LRIT format (tested with N1)
> -   NOAA series, in AAPP, GAC and LAC format (tested with TIROS-N to NOAA-19)
> -   Metop-A/B, in EPS 1a and 1b format
> -   Aqua and Terra MODIS, in hdf-eos format
> -   Suomi NPP, in SDR hdf5 format
> -   TerraSAR-X
> -   Radarsat-2 SAR
> -   COSMO-SkyMed SAR
> -   Sentinel-1 SAR
> -   Sentinel-2 MSI
> -   Sentinel-3 SLSTR & OLCI
> -   FY-3 viir
> -   GCOM-W1 AMSR2 in hdf5 format

See also [satpy documentation pages](http://satpy.readthedocs.io/en/latest) for a list of file formats supported by [satpy](https://github.com/pytroll/satpy).

## Welcome to GitHub Pages

You can use the [editor on GitHub](https://github.com/pytroll/pytroll.github.io/edit/master/index.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/pytroll/pytroll.github.io/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.

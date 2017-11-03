## Workshops

### RSHU, Saint Petersburg, Russia, March 2017

A pytroll developers workshop was held at the Russian State Hydrometeorological University (RSHU) 
in Saint Petersburg, Russia, between March 27th and 31st, 2017. We were around 20 participants from 
various National Meteorological Institutes, universities and companies.

![Pytroll@rshu](https://github.com/pytroll/pytroll.github.io/blob/master/PyTROLL29_small.JPG?raw=true)

### FMI, Helsinki, Finland, November 2016

A pytroll developers workshop was held at the Finnish Meteorological Institute (FMI) in Helsinki between November 
28th and December 2nd, 2016. We were 14 developers from various National Meteorological Institutes and companies 
around Europe.

![Pytroll@fmi](https://github.com/pytroll/pytroll.github.io/blob/master/DSC_4983_small.JPG?raw=true)

### DWD, Offenbach, Germany, June 2016

A pytroll developers workshop was held at the Head Quarters of Deutscher Wetterdienst (DWD) in Offenbach between 
June 13 and 17, 2016. With the paticipation of 18 developers from the national Met Services of Switzerland, 
Norway, Denmark, Sweden, Finland and Germany, as well as EUMETSAT it was the largest to date.

![Pytroll@dwd](https://github.com/pytroll/pytroll.github.io/blob/master/Group2_small.JPG?raw=true)

### MeteoSwiss, Locarno, Switzerland, Dec 2015

Pytroll workshop Locarno 2015

![Pytroll@meteoswiss](https://github.com/pytroll/pytroll.github.io/blob/master/workshop2015december_small.png?raw=true)


### Workshop 2013, November, Norrköping

After a two day open workshop we were 7 pytrollers from Finland, Iceland and Sweden staying till the end of week working 
together on some pressing issues. See below for a summary of achievements. If you would like to contribute actively with 
the pytroll development, please let us know at the mailing list (pytroll@googlegroups.com) or chat with us directly on the 
pytroll slack: https://pytrollslackin.herokuapp.com/. We plan to have two pytroll weeks (usually 4-5 days of dedicated 
programming) each year. Usually we will identifiy a few specific topics that we think needs special attention.

![Pytroll@smhi-2013-1](https://github.com/pytroll/pytroll.github.io/blob/master/00004_tiny.jpg?raw=true)
![Pytroll@smhi-2013-2](https://github.com/pytroll/pytroll.github.io/blob/master/00008_tiny.jpg?raw=true)


#### Summary achievements

 - Extending the user community: Several new users have become more familiar with Pytroll and started contributing.
 - Testing: A number of bugs and user inconveniences were identified, and some have been solved already.
 - Enhancements to Pyresample:
   - Now Pyresample allows to attach a weight to the gaussian reprojection method. This is convenient when e.g. gridding
     several swath products into a level 2.5/3 product (Climate applications).
 - MIPP enhancements and user documentation: MIPP allows XRIT decompression on the fly, and MIPP documentation 
   slightly improved.
 - Three new projects initiated:
   - Pydecorate to add logos, text, color bars and stuff to images
   - Trollimage - an enhancement of the image.py module in mpop including some color enhancements. 
     Will deprecate image.py in mpop
   - Trollduction - A modular batch production framework for Pytroll
 - netCDF reader for SSM/I
 - Trollcast testing, for data exchange between SMHI and FMI - resolution is pending (time outs)
 - Designing and developing the FMI Pytroll based polar production system. Probably resulting in a general concept that can
   be useful to other users
 - Looking at how to enable web based batch production monitoring with Pytroll. Could e.g. be used for an easy and quick access
   to Pytroll products for in-house R&D
 - Initiated an overhaul and check of the EUMETSAT recipe RGBs in Pytroll and how they compare and deviate with the official
   ones. Done in collaboration with the Romanian Met Service.
 - Colorizing Pytroll images (using the new trollimage component) - "sandwich" product. Color enhanced imagery is commonly
   used in forecast offices, e.g. IR imagery with cold temperatures enhanced using a color palette.



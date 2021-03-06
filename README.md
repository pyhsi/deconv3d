
WHAT IS IT
==========

**This is a work in progress.**

This is an implementation of a MCMC for estimation and non-parametric
deconvolution of galactic kinematics from hyperspectral data cubes.

It is a python `2.7` module designed to be flexible, reliable and fast.
It has not been tested under python `3.x`, but feel free to make it compatible !


HOW TO INSTALL
==============

Using pip
---------

_(still not available)_

Install `deconv3d` system-wide,

```
$ sudo pip install deconv3d
```

or just for you :

```
$ pip install --user deconv3d
```

Running one of the above commands will download and install the module on
your system, as `deconv3d` is referenced on the official [python package index]
(https://pypi.python.org).



Manually
--------

_(still not available)_

Running `python setup.py install` should do the trick.


Mandatory Dependencies
----------------------

- `astropy` : http://www.astropy.org
- `hyperspectral` : https://pypi.python.org/pypi/hyperspectral
- `matplotlib` : https://pypi.python.org/pypi/matplotlib


Optional Dependencies
---------------------

- `bottleneck` : https://pypi.python.org/pypi/Bottleneck


DEBIAN PACKAGES
---------------

Most of the usual packages can be installed system-wise from repositories.

```
python2.7 python-numpy python-astropy python-matplotlib
```

You can also install them via `pip`, it's your choice.


MPDAF PACKAGES
--------------

_Optional._

`deconv3d` provides a `MUSELineSpreadFunction` class that depends on
`mpdaf.MUSE.LSF`.

Follow [MPDAF install instructions]
(http://urania1.univ-lyon1.fr/mpdaf/chrome/site/DocCoreLib/installation.html).

`deconv3d` also accepts `MPDAF`'s Cubes as input.


HOW TO TEST
===========

Simply run `nosetests -v --nocapture --nologcapture` from project's root :

- `-v` is verbose
- `--nocapture` means `print` statements will print
- `--nologcapture` means `logging` statements will print

These options are not mandatory for the tests to pass, but they are useful.

If you don't have `nose`, you can either

    $ apt-get install python-nose

or

    $ pip install --user nose


HOW TO DOCUMENT
===============

Install sphinx :

    $ apt-get install python-sphinx

Make your changes into the `doc/source` files.

Once its done, go to `doc` directory, run `make html`.


HOW TO CONTRIBUTE
=================

Get the sources.

Create a virtualenv with python 2.7 :

    $ virtualenv venv2.7 -p /usr/bin/python2.7

Activate that virtualenv :

    $ source venv2.7/bin/activate

Install dependencies :

    $ pip install -r requirements.txt

You're ready to run the test-suite !


ACRONYMS
========

_Real geniuses never define acronyms. They understand them genetically._

 Acronym | Meaning
---------|----------------------------------------------------------------------
EAFP     | Easier to Ask for Forgiveness than Permission
FFT      | Fast Fourier Transform
FITS     | Flexible Image Transport System
FWHM     | Full Width at Half Maximum
HDU      | Header Data Unit
LBYL     | Look Before You Leap
LSF      | Line Spread Function
MCMC     | Markov Chain Monte Carlo
MH       | Metropolis-Hastings
MPDAF    | MUSE Python Data Analysis Framework
MUSE     | Multi Unit Spectroscopic Explorer
NFM      | Narrow Field Mode
PA       | Position Angle
PC       | ParseC
PSF      | Point Spread Function
SNR      | Signal to Noise Ratio
WCS      | World Coordinates System
WFM      | Wide Field Mode

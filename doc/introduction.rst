.. _introduction:

An introduction to seaborn
==========================

Seaborn is a library for making attractive and informative statistical graphics
in Python. It is built on top of `matplotlib <https://matplotlib.org/>`_ and
tightly integrated with the `PyData <https://pydata.org/>`_ stack, including
support for `numpy <http://www.numpy.org/>`_ and `pandas
<https://pandas.pydata.org/>`_ data structures and statistical routines from
`scipy <https://www.scipy.org/>`_ and `statsmodels
<https://www.statsmodels.org/>`_.

Some of the features that seaborn offers are

- Several :ref:`built-in themes <aesthetics_tutorial>` for styling matplotlib graphics
- Tools for choosing :ref:`color palettes <palette_tutorial>` to make beautiful plots that reveal patterns in your data
- Functions for visualizing :ref:`univariate <distplot_options>` and :ref:`bivariate <joint_kde>` distributions or for :ref:`comparing <grouped_violinplots>` them between subsets of data
- Tools that fit and visualize :ref:`linear regression <anscombes_quartet>` models for different kinds of :ref:`independent <pointplot_anova>` and :ref:`dependent <logistic_regression>` variables
- Functions that visualize :ref:`matrices of data <heatmap_annotation>` and use clustering algorithms to :ref:`discover structure <structured_heatmap>` in those matrices
- A function to plot :ref:`statistical timeseries <timeseries_from_dataframe>` data with flexible estimation and :ref:`representation <timeseries_bootstrapped>` of uncertainty around the estimate
- High-level abstractions for structuring :ref:`grids of plots <faceted_histogram>` that let you easily build :ref:`complex <many_facets>` visualizations

Seaborn aims to make visualization a central part of exploring and
understanding data. The plotting functions operate on dataframes and arrays
containing a whole dataset and internally perform the necessary aggregation and
statistical model-fitting to produce informative plots. If matplotlib "tries to
make easy things easy and hard things possible", seaborn tries to make a
well-defined set of hard things easy too.

The plotting functions try to do something useful when called with a minimal
set of arguments, and they expose a number of customizable options through
additional parameters. Some of the functions plot directly into a matplotlib
axes object, while others operate on an entire figure and produce plots with
several panels. In the latter case, the plot is drawn using a Grid object that
links the structure of the figure to the structure of the dataset.

Seaborn should be thought of as a complement to matplotlib, not a replacement
for it. When using seaborn, it is likely that you will often invoke matplotlib
functions directly to draw simpler plots already available through the
``pyplot`` namespace. Further, the seaborn functions aim to make plots that are
reasonably "production ready" (including extracting semantic information from
Pandas objects to add informative labels), but full customization will require
changing attributes on the matplotlib objects directly. The combination of
seaborn's high-level interface and matplotlib's customizability and wide range
of backends makes it easy to generate publication-quality figures.

The documentation is divided into three separate domains. The breadth of
functionality offered by the package is demonstrated in a set of short scripts
and rendered in the :ref:`example gallery <example_gallery>`. Some motivation
behind the kind of plots that seaborn can help to make is explained in the
:ref:`tutorial <tutorial>`. Authoritative documentation on the options afforded
by each function and class can be found by consulting the :ref:`API reference
<api_ref>`.


---
layout: page
title: Introduction to OpenDA
---
OpenDA is a generic environment for data-assimilation tasks like parameter calibration and measurement filtering. It provides a platform that allows an easy interchange of algorithms and models.

It is a modular framework, containing methods and tools that can be used for a wide range of applications. By offering the data-assimilation software as a separate component, the cost of applying data-assimilation methods in one's project is reduced. At the same time, it allows new developments in the field of data assimilation to quickly spread to all applications that might benefit from it. A short introduction to data assimilation can be found [here](https://openda-association.github.io/wiki/introduction_da).

OpenDA is configured using [XML files](https://en.wikipedia.org/wiki/XML) (Extensible Markup Language files), in which the information about the data-assimilation components is specified. For instance, if you would like to use a different calibration algorithm or stochastic observer, or if you would like to couple your own model to OpenDA, you should provide all necessary settings, file names, variable names etc. to OpenDA in XML input files. The format of the XML files is specified in [XML schema files](https://en.wikipedia.org/wiki/XML_schema) (`.xsd`) that are hosted on the [OpenDA website](http://openda.org/docu/openda_2.4/doc/xmlSchemasHTML/index.html). The diagrams describing the format of the XML schemas can be found there as well. 

In general, the user needs to provide one main configuration file and a number of configuration files describing each data-assimilation component. The main configuration file contains references to the other components’ configuration files. Usually, there are three main data-assimilation components: stochastic model, stochastic observer, and algorithm. In addition, another component may be specified to configure how OpenDA output will be stored. 

For more information about the configuration files, click [here](https://openda-association.github.io/wiki/configuration_files).

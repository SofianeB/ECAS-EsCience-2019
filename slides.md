
Data Analysis and Sharing with the ENES Climate Analytics Service
=================================================================

<img src="images/ecas_logo.png" height="90" width="490" alt='ECAS' style="border: 0">

**Sofiane Bendoukha** 

German Climate Computing Center (DKRZ)

eScience 2019 15th International Conference

24-27 September, San Diego, USA

<img src="images/eoschub_logo.png" width="50" alt='ECAS' style="border: 0">  <img src="images/eu.png" width="50" alt='ECAS' style="border: 0"> <br/> <small> EOSC-hub receives funding from the European Union's Horizon 2020 research and innovation programme under grant agreement No. 777536 </small>


---

Agenda
======

* ECAS presentation 
* Demo
* Hands on 
* Exercise
* Break (Lunch) 
* Data sharing with ECAS
* ECAS & WPS (optional) 
* Wrap up


***

About Me/Us
===========

* Sofiane Bendoukha
  * bendoukha@dkrz.de
* Pre-DKRZ
  * (Scientific) workflow management systems
  * Grid / Cloud computing
  * Service orchestration 
  * Workflow modeling
* Joined DKRZ in January 2017
  * **Climate** data management 
  * Software tools, computing gateways for climate community 

---

### German Climate Computing Center

<img src="images/dkrz_logo_mit_unterzeile.png" width="120" alt='ECAS' style="border: 0">

* Hamburg, Germany, www.dkrz.de
* Supports projects related to 
  * preparation 
  * quality assessment, 
  * distribution and
  * long-term archiving of data

---

### German Climate Computing Center

<img src="images/dkrz_logo_mit_unterzeile.png" width="120" alt='ECAS' style="border: 0">
* Provides high performance computing (HPC) platforms, sophisticated and high capacity data management and services for premium climate science.
* HLRE-3 "Mistral" Supercomputer

  * 3.300 compute nodes
  * 100.000 compute cores 
  * 266 Terabytes of memory and
  * 54 Petabytes of disk
  * HLRE-4 coming soon ...
 
<img src="images/HLRE-3.jpg" width="450" alt='ECAS' style="border: 0">
 
***

Tutorial Materials
==================

* Slides
https://statiksof.github.io/ECAS-EsCience-2019/slides/

* Notebooks
https://github.com/ECAS-Lab/ecas-training/

---

Useful Links
============

* ECASLab Web site 
https://ecaslab.dkrz.de

* Jupyterhub 
https://ecaslab.dkrz.de/jupyter/

* Ophidia user documentation
http://ophidia.cmcc.it/documentation/users/index.html


***

**ENES Climate Analytics Service**
==================================

<img src="images/ecas_logo.png" height="100" width="495" alt='ECAS' style="border: 0">


---

The European Open Science Cloud
-------------------------------

<img src="images/eosc.png" height="455" width="695" alt='EOSC' style="border: 0">

https://eosc-portal.eu/

---

### EOSC-hub project 

<img src="images/eosc-hub.png" width="750" alt='EUDAT' style="border: 0" hspace="50" />
 
* EC H2020 Project 
* Under the coordination of **EUDAT**, **EGI** and **INDIGO-DataCloud**
* The catalogue includes services in four broad areas: Common, Thematic, Collaborative and Federation.
* Training activities


<small> EOSC-hub receives funding from the European Union's Horizon 2020 research and innovation programme under grant agreement No. 777536 </small>

---

Overview
--------

* **ECAS** is part of **WP 7**: thematic services
  * **ECAS** enables scientific end-users to perform data analysis experiments 
* Server-based 
  * Computation **@ DKRZ** or **CMCC**
  * Avoid data transfer (download)
  * Improved reusability of data and workflows (**FAIR approach**)
* **ECAS** supports different Auth* providers 
  
  * Local and external providers supported (**LDAP**, **B2ACCESS**, **EGI Check In**)  
  * Additional AAI providers can be integrated on demand (e.g. **GITHUB**) 
  
---

#### Service Architecture and Interfaces

<img src="images/new_ecas_architecture.png" height="455" width="695" alt='ECAS Architecture' style="border: 0">

---


### Data overview 
<img src="images/esgf.png" height="80" width="470" alt='ECAS' style="border: 0">

* ECAS provides data access via ESGF
* Coordinated Regional Climate Downscaling Experiment
  * ~ 100 Tbyte Cordex
* Coupled Model Intercomparison Project 5
  * ~ 1.2 Pbyte CMIP 5 data
* Coupled Model Intercomparison Project 6
  * ~ 250 Tbyte CMIP6 data from the 1PByte published
* Other data pools can be mounted on demand 
  * MPI Grand Ensemble (**MPI-GE**)
  * Data collection exposed in the Federated Data Archive (e.g. **OneData**) 

---

Ophidia framework overview
--------------------------

[ophidia.cmcc.it](http://ophidia.cmcc.it)

* The Ophidia framework addresses big data chellenges for eScience
  * support for declarative, parralel, server-side data analysis exploiting parralel computing techniques 
  * end-to-end mechanisms tu support complex experiments and large processing workflows on scientific multi-dimensional cubes 
* Ophidia supports both **batch** and **interactive** data analytics 
  * More than 50 datacube-oriented **operators** are available, including: data reduction and subsetting, data intercomparison, metadata and provenance management, 
    time series analysis with array-based primitives
  * A wide set of (low-level) array-based primitives (over 100) to perform, e.g. data summerization, algebraic expressions, predicates evaluation, statistical analysis
  * Support for complex workflows ad Python applications execution 

<img src="images/oph_logo_symbol_big.png" width="100" alt="Ophidia" style="border: 0">

---

#### Server-side paradigm and datacube abstraction in Ophidia

<img src="images/ophidia.png" height="455" width="700" alt="Ophidia" style="border: 0">

---

ECASLab 
-------

<img src="images/ecaslab.png" height="480" width="750" alt="Ophidia" style="border: 0">

---

Data sharing with ECAS
----------------------

* Share your results with your team or with researchers from a broader community 
  * Post-processing datasets
  * Jupyter notebooks
* Cloud-based storage and sharing services integrated within ECAS
  * **B2DROP** online storage for external/internal collaborators. 
    Keep data synchronized and up-to-date  
  * **B2SHARE** store and publish research data from diverse contexts. Data assigned a **Persistent Identifiers** for better findability  
  * **DataHub (OneData)** a global data access solution for eScience 

<img src="images/logo-b2drop.png" height="50" width="70" alt="b2drop" style="border: 0"> &nbsp;&nbsp; <img src="images/b2share.png" height="48" width="70" alt="b2share" style="border: 0"> &nbsp;&nbsp; <img src="images/onedata.png" height="40" width="100" alt="onedata" style="border: 0">

***

***

Demo
====


---

### Register/Log in and explore the Jupyter environment

When you log in to JupyterHub, a workspace is created for you with following directories:

* **/data**: input data required for the workflows/notebooks
* **/notebooks**: set of ready-to-use Jupyter Notebooks with the implemented use cases
* **/workflows**: script-based workflows
* **/quickstart**: quick guide showing how to use JupyterHub and instantiate terminals in ECASLab

---

Notebooks
=========

All notebooks are available in **/notebooks** directory in your jupyter workspace.

* Subsetted map (.ipynb)
* Tropical nights (.ipynb)
* Time Series Difference (.ipynb)

---

Terminal 
========

* The Ophidia Terminal is a robust, comprehensive, effective and extremely usable client, developed with characteristics similar to the bash program present in almost all Unix-like environments. 
* In fact, besides submitting the Ophidia operators, it provides history management, embedded command help/manual, operator/command auto-completion, aliases creation and output rendering features.
* This demo will show examples of usage of the Ophidia Terminal and its main capabilities.

---

Hands on
========

<br/>
* Open the following notebook: 
  **/notebooks/ECASLab-Training.ipynb**
* It provides step-by-step instructions on how to use the Ophidia operators as well as the PyOphidia library.
* After the completion you can try to run the other notebooks available under the /notebooks folder or proceed with the following exercise.


---

Exercise
========

* Calculate the number of Summer days 
* Starting from the daily maximum temperature, the Summer Days index is the annual count of days number of days where TX (daily maximum temperature) > 25°C
* Based on the definition, try to calculate the number of Summer Days (you can start from the Tropical_Nights.ipynb notebook).
* Useful information: 
  * Input NetCDF:

    * E63_kp40_198001_199012_T2m_daymax_merged.nc

    * tasmax_day_CMCC-CESM_rcp85_r1i1p1_20960101-21001231.nc

  * 25°C: 298.15 Kelvin

---

## Break?

---

## Data Sharing with ECAS

* Store and sync your data with B2DROP
* Share and publish your result with B2SHARE

---

## EUDAT B2DROP

* B2DROP shared
  * no log in required 
  * https://b2drop.eudat.eu/s/gDyJjMeJ2Xiapwi

* B2DROP private 
  * initial 20 GB for each user
  * mounted in you user workspace

---

## EUDAT B2SHARE

![](https://github.com/SofianeB/ECAS-B2SHARE/raw/master/demo-ecas-ophidia/ecas-b2share.png)

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/SofianeB/ECAS-B2SHARE/master?filepath=demo-ecas-ophidia%2Fecas-b2share.ipynb) 

---

## ECAS & WPS (Optional)

* Provide ECAS workflows as web services 
* Switch the JupyterHub profile and start ECAS-Birdhouse
 

***

Wrap up 
=======

* Q & A
* collect forms

---

Stay in touch!
==============

* Support
ecas-support@dkrz.de
* Chat
https://gitter.im/ECAS-ECASLab/Lobby
# Data Analysis and Sharing with ECAS

## Tutorial on ECAS at eScience 2019, San Diego, CA, USA

Trainer: **Sofiane Bendoukha**

Wed, 25 Sept, 10:30 AM – 2:30 PM Room *Boardroom East* 


The ENES Climate Analytics Service (ECAS) enables scientific end-users to perform data analysis experiments on large volumes of climate data, by exploiting a PID-enabled, server-side, and parallel approach.

It aims at providing a paradigm shift for the European Network for Earth System Modelling (ENES) community with a strong focus on data intensive analysis, provenance management, and server-side approaches as opposed to the current ones mostly client-based, sequential and with limited/missing end-to-end analytics workflow/provenance capabilities.


## Agenda


* ECAS presentation 
* Demo
* Hands on 
* Exercise
* Break  
* Data sharing with ECAS
* ECAS & WPS (optional) 
* Wrap up

---
**Note**

The presentation slides can be found [here](https://statiksof.github.io/ECAS-EsCience-2019/)

---

## Organization

* Please fill in the evaluation forms at the end of the tutorial and give them back to the trainers.

* To [log in](https://ecaslab.dkrz.de/jupyter/), please use the credentials that you received when you registered.

---
**NOTE**

If you have not registered yet, ask the organizers for a default account.

---

## Setup / useful links

**ECAS Portals**

- https://ecaslab.dkrz.de

**ECASLab / JupyterHub** 

- https://ecaslab.dkrz.de/jupyter/

**Documentation**

- [Ophidia framework documentation](http://ophidia.cmcc.it/documentation/users/index.html)
- [ECAS documentation](https://ee-docs.readthedocs.io/en/latest/)

**Github**

- https://github.com/ECAS-Lab
- https://github.com/OphidiaBigData/PyOphidia


## Explore the Jupyter environment

When you log in to JupyterHub, a workspace is created for you with following directories:

- **/data:** input data required for the workflows/notebooks
- **/notebooks:** set of ready-to-use Jupyter Notebooks with the implemented use cases
- **/workflows:** script-based workflows
- **/quickstart:** quick guide showing how to use JupyterHub and instantiate terminals in ECASLab


## Demo

### 1. Notebook

All notebooks presented during the demo are available under the **/notebooks** directory in your jupyter workspace.

1. *Subsetted map (.ipynb)*
2. *Tropical nights (.ipynb)* 
3. (Optional) *Time Series Difference (.ipynb)*

### 2. Terminal

The Ophidia Terminal is a robust, comprehensive, effective and extremely usable client, developed with characteristics similar to the bash program present in almost all Unix-like environments. In fact, besides submitting the Ophidia operators, it provides history management, embedded command help/manual, operator/command auto-completion, aliases creation and output rendering features. 

This demo will show examples of usage of the Ophidia Terminal and its main capabilities.

## Hands on

The following notebook cover more details on data processing operations using ECAS/Ophidia:

**Notebook** ECASLab-Training.ipynb

It provides step-by-step instructions on how to use the Ophidia operators as well as the [PyOphidia](https://github.com/OphidiaBigData/PyOphidia) library.

After the completion you can try to run the other notebooks available under the **/notebooks** folder or proceed with the following exercise.


## (Short) Exercise 

Starting from the daily maximum temperature, the Summer Days index is the annual count of days number of days where TX (daily maximum temperature) > 25°C

Based on the definition, try to calculate the number of Summer Days (you can start from the *Tropical_Nights.ipynb* notebook).

Useful information:

**Input NetCDF:** Same as *Tropical Nights* notebook

**25°C:** 298.15 Kelvin

---
**NOTE**

Once completed you can compare your implementation with the *Summer Days* notebook provided under the **/notebooks** folder. 

---

## Share your datasets / workflows

Now, you are going to learn how to you can share your results (datasets, notebooks) with other ECAS users. 

* Store / Sync your data with B2DROP
  * shared link https://b2drop.eudat.eu/s/gDyJjMeJ2Xiapwi
  * directory in your workspace **b2drop-shared**
* Share and publish your results with B2SHARE (Beta)
  * ecasb2share Python library 
  * create records with assigned persitent identifiers 
  * add files to created record
  * publish records 

---

## Wraps Up

+ Access and Log in to *ECAS/ECASLab*
+ Compute climate indices
+ Visualize results
+ Share results 

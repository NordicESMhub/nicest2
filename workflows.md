---
layout: page
title: ESM workflow tools
description: Earth System Modelling workflow management tools for improved performance
background: '/img/workflows.png'
---

> ### Table of content
> {:.no_toc}
> 1. TOC
> {:toc}
>
{: .agenda}

# Objectives

- Ease the building of Reproducible Workflows for Earth System Modelling Systems.
- Enhance the performance and optimize and homogenize workflows used, so climate models (like EC-EARTH and NorESM) can be run in an efficient way on future computing resources (like EuroHPC).

[A short video explaining what the "Common Workflow Language" is in 64 seconds](https://youtu.be/86eY8xs-Vo8)

## ESM workfows to efficiently run NorESM and ECEarth on euroHPC

As part of this Work Package we investigate the use of workflows to improve reproducibility and automation of a sequence of tasks 
required for running an Earth System Model on various computing platforms, perform data processing, create graphs, etc.
As an example a simple workflow was developped on Galaxy Climate with FATES, the Functionally Assembled Terrestrial Ecosystem 
Simulator which is part of the Community Terrestrial Systems Model (CTSM). 
The tasks involve:
- preparing the input data (plus in this instance restart files from a previous experiment)
- setting-up the simulation, compiling the code and running the simulation on Galaxy (using a CTSM/FATES tool/container)
- extracting relevant variables from the output files
- making a scatter plot (time series of the total carbon in live plant leaves)
This workflow being stored on WorkflowHub allows other people to easily reproduce the same numerical experiment out-of-the-box, 
and also make changes, explore other options, alter the data processing or plots, etc.

Each task in such workflows rely on containers, and work in this area has also progressed with Docker container images developed 
(both with the homemade GCC toolchain and using "standard" packages from conda-forge/bioconda) and successfully tested with 
CESM/NorESM on Virtual Machines from the Norwegian Research and Education Cloud (NREC), on the Google Cloud Platform (GCP)
and on Personal Computers (all multiple cores single node applications). This kind of container is particularly suited for training
and model development purposes for which using a High Performance Computer (HPC) would be a waste of resources.
Singularity is now available on HPCs from Sigma2 (Saga, Fram and Betzy), and our next challenge will be
to develop portable containers to carry out tests with multiple nodes and assess the performance of containerized applications 
compared to "bare metal" (ran directly on the host).

# Outputs of the projects

- [NICEST2 WP4: Update about ESM workfows to efficiently run NorESM/CESM and EC-Earth on euroHPC](https://doi.org/10.5281/zenodo.4635687) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4635687.svg)](https://doi.org/10.5281/zenodo.4635687)

## Task 4.1 (Sigma2/UiO, NORCE, NERSC, FMI): Reproducible workflows for deploying and running ESM on future HPCs (M4 – M30)

- [NordicESMhub/eosc-nordic-jupyterhub: v0.8.2 JupyterHub conda environments for the NIRD toolkit](https://doi.org/10.5281/zenodo.4626757) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4626757.svg)](https://doi.org/10.5281/zenodo.4626757)

- [NordicESMhub/container-noresm: Version 2.0.0 NorESM container for running on HPC with singularity](https://doi.org/10.5281/zenodo.4670215) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4670215.svg)](https://doi.org/10.5281/zenodo.4670215)

- [NordicESMhub/noresm-containers-timings: Jupyter notebook for plotting timings from NorESM/CESM simulations](https://doi.org/10.5281/zenodo.4670175) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4670175.svg)](https://doi.org/10.5281/zenodo.4670175)


## Task 4.2 (NORCE, Sigma2/UiO, FMI): Efficiency of Nordic ESMs on future euroHPC (M4 – M36)

- [Final results from the CSC GPU hackathon for NorESM/NICEST2](https://doi.org/10.5281/zenodo.4719793) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4719793.svg)](https://doi.org/10.5281/zenodo.4719793)

- Our first report on the identified bottlenecks for an efficient usage of Nordic ESMs on EuroHPC is now available [online](https://doi.org/10.5281/zenodo.4749515). [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4749515.svg)](https://doi.org/10.5281/zenodo.4749515)


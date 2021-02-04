---
layout: page
title: ESM workflow tools
description: Earth System Modelling workflow management tools for improved performance
background: '/img/workflows.png'
---

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

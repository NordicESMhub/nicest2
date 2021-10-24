---
layout: post
title: "NICEST2 Status, progress and challenges"
subtitle: "23th October 2021"
date: 2021-10-23
background: '/img/posts/bernd-klutsch-nE2HV5AUXFo-unsplash.jpg'
---

In this post, you will learn about the NICEST2 project status & updates.

#### Authors:
- Anne Fouilloux, Project Manager
- Oskar Landgren, WP2 Leader
- Hamish Struthers, WP3 Leader substitute
- Jean Iaquinta, WP4 Leader

## WP2: Model analysis and diagnostics focused on the Nordic regions

- Task 2.1 (MET Norway, NERSC): Organization of workshop/hackathon at the beginning of the project on ESMValTool to collect user requirements (M3 – M9)
	- Workshop held March 12, 2021. Report available (deliverable 2.1) online.
	- Serves as input to Task 2.2.
- Task 2.2 (FMI, MET Norway, NERSC): Development of new ESMValTool diagnostic modules for the Nordic regions (M7 – M24)
	- Started. User group established.
- Task 2.3 (NERSC, MET Norway, FMI, Sigma2/UiO): Development of teaching material for learning how to use ESMValTool diagnostics over the Nordic regions (M18 – M36)
	- Not yet started

### Task 2.1: Workshop held on March 12, 2021 'Nordic ESM diagnostics hackathon'

- Collaboration between NICEST2, INES and IS-ENES3 projects.
- Programme:
	- Introduction to ESMValTool
	- Roundtable discussion: Tools and analyses currently in use at each institute
	- Nordic hub for joint evaluation of ESMs
	- Three working groups:
		- How can the ESMValTool be used in Nordic cooperation projects? How to do efficient multi-model evaluations across groups?
		- User needs for a Nordic climate evaluation module for ESMValTool. Regionally specific indices etc.
		- Quicklook diagnostics for NorESM development
	- Hands-on session for new users to try ESMValTool on NIRD

#### Outcomes:

- Improved Nordic collaboration on ESM intercomparison
- Survey about ESM analysis tools used organised
- User group for Nordic ESMValTool recipes established
- Event on CMORization organised (June 8)

### WP2: Current work

#### Organisation of T2.2:

- Discussions on NEIC Slack channel
- Collaboration on ESMValTool: 
	- Collect scripts/diagnostics (google form) 
	- Online workshop in December

## WP3: FAIR climate data for NorESM and EC-Earth

<img src="https://nordicesmhub.github.io/nicest2/img/posts/WP3_dow.png" width="800"/>

### Task 3.1 - Support for Nordic ESGF hosting of CMIP6 data

- **Success**: Support Nordic ESGF operations.

<img src="https://nordicesmhub.github.io/nicest2/img/posts/esgf-1.png" width="800"/>

- **Challenge**: How to widen to collaboration/participation/interest in ESGF operations. 

<img src="https://nordicesmhub.github.io/nicest2/img/posts/esgf-2.png" width="700"/>

- **Future of ESGF?**

A large part of CMIP6 datasets is already available as Zarr, a cloud-optimized format. In this context, where end-users would like to have both access and computing resources to manipulate and analyze data, it is unclear if ESGF (as it is now) will be pursued in the future.

<img src="https://nordicesmhub.github.io/nicest2/img/posts/esgf-3.png" width="600"/>

### Task 3.2 -  Towards FAIR Nordic climate modeling data 


<img src="https://nordicesmhub.github.io/nicest2/img/posts/fair-1.png" width="700"/>

- **Success**: Workshop held on March 11, 16 & 17, 2021 'NICEST2 FAIR climate data hackathon'
	- Collaboration between NICEST2 and EOSC-Nordic projects.
	- 29 registrations received.
	- Deliverable 3.3:[Report on NICEST2 FAIR climate data hackathon](https://doi.org/10.5281/zenodo.4944686)
	- Three focus areas:
		- FAIR data cookbook for climate
		- Idealized citation
		- Ontologies

- **Challenges**: Sustainable engagement with researchers
	- User reference group?
		- Researcher: “What do I get from this?”
	- Outreach: Training & workshops
	- Identification and support for early adopters (champions)
	- **Lesson**: considerable effort is required in follow-up to sustain the initial momentum from workshops/hackathons.


<img src="https://nordicesmhub.github.io/nicest2/img/posts/fair-2.png" width="500"/>

## WP4 - Earth System Model Workflows

*The primary objective of the work package is to develop expertise on how to run efficiently ESM workflows and facilitate the porting and deployment of ESMs used in Nordic countries (CESM, NorESM & EC-Earth) on future HPCs, in particular the EuroHPC.*


- **Task 4.1**: Reproducible workflows to deploy and run ESMs on future HPCs
	- Workflow Management Systems 
	- Packaging & containers

- **Task 4.2**: Efficiency of Nordic ESMs on future euroHPC
	- Common workflow for performance analysis of Nordic ESMs
	- Best practices & what needs to be done to run on EuroHPC

### Task 4.1 - Achievements

- Galaxy was selected after assessing practices & needs (Deliverable 4.1)
	- Supports a wide range of users with different levels of expertise
	- Comes with a Graphical Workflow Editor
<img src="https://nordicesmhub.github.io/nicest2/img/posts/wp4-1.png" width="800"/>
	- Can interoperate with other WMSs and will be CWL compatible
	- Accommodates metadata

→ Talks ([ESMaaS](https://youtu.be/o8lSkZvuW9A?t=360) & teaching material ([Reproduce published analyses](https://training.galaxyproject.org/training-material/topics/introduction/tutorials/galaxy-reproduce/tutorial.html).

- Packaged ESMs for easy installation (conda) and containerization
	- Facilitates porting on diverse infrastructures (PC, cloud, HPC)
	- Releases HPC resources (more suited for production)
	- Similar recipes work for CESM/NorESM & EC-Earth
	- Leverages native performances and provides BFB reproducibility

→ Will be introduced to NorESM users ([2021 workshop](https://nordicesmhub.github.io/NorESM_user_workshop_2021).

### Task 4.2 - Achievements


- Successfuly ran containerized ESMs on HPC and HPC-cloud
	- Fram/Betzy@Sigma2, PizDaint@CSCS, Puhti@CSC, NREC/GCP/OCI
<img src="https://nordicesmhub.github.io/nicest2/img/posts/wp4-2.png" width="700"/>
	- Preparing LUMI Pilot (testing on Eiger@CSCS in the meantime)

- Defined real-world cases & simulation parameters for benchmarking
	- Collecting performance figures for reference (NorESM performance)

- Identified bottlenecks for an efficient usage of Nordic ESMs on EuroHPC
	- GPU Hackathon@CSC ([Deliverable 4.5](https://doi.org/10.5281/zenodo.4749515))

- Container recipes usable for other CPU architectures than Intel & Amd
	- PowerPC (IBM) & ARM (OCI, eX3@Simula, LightHPC@UiO) 

## WP1 - Management

- Organization:
	- Monthly project meetings
- Deliverables
	- Quality control for deliverables: internal review (from someone outside WP), then PM/PO and then SG
	- Published in zenodo: 
		- [NICEST2 - D3.3](https://zenodo.org/record/4944686): Report on NICEST2 FAIR climate data hackathon (M9)
		- [NICEST2 - D4.5](https://zenodo.org/record/4749515): First report on the identified bottlenecks for an efficient usage of Nordic ESMs on EuroHPC (M9)
		- [NICEST2 - D2.1](https://doi.org/10.5281/zenodo.5571344): "Report on the workshop/hackathon to discuss about how to use ESMValTool with a focus on the Nordic countries and collect user requirements for the two training materials"  (M12)
		- [NICEST2 - D4.1](https://doi.org/10.5281/zenodo.5571416): "Identification of the Nordic ESM community needs for ESM workflows" (M12)


### Next steps for WP1

#### Improve communication

- Post regular training & events on NordicESMHub website
	- https://nordicesmhub.github.io/events: see upcoming trainings on Python and OpenMP/LUMI
	- Send message to PM to add new events
- Improve internal and external communication
	- More regular newsletters & highlights
	- Follow-up after training/hackathons to sustain collaboration effort
	- Organize Open hour for everyone (1 hour one per month)
		- Ask any questions about NICEST2
		- Present/record info about progress, how to, showcases e.g. show your diagnostics, use jupyter notebook on EOSC to visualize CMIP6 data, run norESM with a container, etc.


---
layout: post
title: "NICEST2 newsletter"
subtitle: "20th April 2021"
date: 2021-04-20
background: '/img/posts/newsletter.png'
---

> ### Agenda
> {:.no_toc}
> 1. TOC
> {:toc}
>
{: .agenda}

Download [NICEST2 newsletter in PDF format](/nicest2/img/posts/2021-04-NICEST2Newsletter.pdf)

## Project status and updates

### A glossary for mutual understanding

Improving Earth System Models require expertise by scientists from different disciplines and practitioners working together. Recent experience, for instance during the GPU hackathon, showed that some words are commonly used by the Nordic ESM community but often unknown or have a different meaning by GPU specialists. 

To clarify and ease collaboration, the NICEST2 project will work on creating a glossary of terms used within the Nordic Earth System Modelling Community. A first draft is available [online](https://github.com/NordicESMhub/nordic-climate-glossary) and we will organize an hackathon to work together on a list of common definitions.

### Lesson learned from the hackathon on ESMValTool

The hackathon on ESMValTool, organized by INCES, NICEST2 and IS-ENES3, was held on 12 March 2021. 25 people participated (out of 27 signed up) from four Nordic countries: Denmark, Finland, Norway and Sweden.
The hackahton was "divided" in two parts with a series of talks in the morning and discussions and hand-on in the afternoon.

#### Goals

- Collect user requirements for diagnostic tools (ESMValTool, NCAR diagnostics, pyaerocom etc.) to support ESM model development in the Nordic countries (NorESM, EC-EARTH, ...).
- Exchange on current possibilities to use the ESMValTool and other tools on Nordic computing platforms in an efficient way.
- Explore ideas on developing a climate diagnostic ESMValTool module for the Nordic regions.
- Discuss other tools to enhance diagnostic capabilities (CMORization of model output on the fly for easy use of ESMValTool & other diagnostic libraries, Quicklooks for model development), multi-model evaluation scripts for CMIP6 analysis.

#### Outcomes

- Many people got their first introduction to ESMValTool with a practical session in the afternoon to try it out. Testing ESMValTool in EOSC-Nordic Jupyterhub collaborative platform before hands-on session uncovered some issues and led to improvements in documentation.
- Discussion of current use of diagnostics at different Nordic Meteorological institutes showed that a large variety of ad-hoc tools are being used.
- The use of ESMValTool in Nordic cooperation projects is still limited but everyone showed an interest in increasing synergies in future cooperations. A NeIC Slack channel was then established as a low-threshold communication platform. Please contact annefou-at-uio-no if you wish to be invited to the slack channel.
- User needs for Nordic climate evaluation module were collected and will serve as inputs for NICEST2 WP2.

### Lesson learned from the hackathon on FAIR climate data

Three half-days (12, 16-17 March) event organized by NICEST2. The hackathon was divided in presentations, discussions and practical work. The full program is available [here](https://nordicesmhub.github.io/nicest2-fair-hackathon). 19 people participated from Norway(10), Sweden(5), South Africa(2), France(1), US(1).

#### Goals

- Explore how the current international standards and tools for managing climate model output (including [ES-DOC](https://es-doc.org/), [CF-conventions](https://cfconventions.org/), [ACDD](https://wiki.esipfed.org/Attribute_Convention_for_Data_Discovery_1-3), [CMOR](https://cmor.llnl.gov/), [ESGF](https://esgf.llnl.gov/), etc.) can be reused in Nordic and national research projects to help ensure the valuable climate model outputs are FAIR and open.
- Look at real-world output from global climate models (NorESM and EC-Earth), and how to generate comprehensive metadata from raw model simulation output.
- Understand how metadata generation fits into the research workflow
- Discuss the role of data management as a help to FAIRification.

#### Outcomes

- Lots of useful/interesting input in HackMD doc. from participants during hackathon. We still have lots of information to process and publish!
- All the presentations are available on the NordicESMHub YouTube channel (see the [agenda day-1](https://nordicesmhub.github.io/nicest2-fair-hackathon/day1-agenda/) and [agenda day-2](https://nordicesmhub.github.io/nicest2-fair-hackathon/day2-agenda/)).
	- [Introduction to Open Science and FAIR data](https://youtu.be/5BrzbdRBRFM)
	- [Data management planning and data life cycle](https://youtu.be/JWzzR_RlcN4) - perspective of a data manager
	- [Climate researchers perspective](https://youtu.be/lWqcN3IR9oE)
	- [ES-DOC](https://youtu.be/sF50iFZzzmI) (1 hour)
		- [Introduction/high level overview of ES-DOC](https://github.com/NordicESMhub/nicest2-fair-hackathon/blob/main/content/presentations/es-doc-for-cmip6-intro.pdf) (Sadie Bartholomew, NCAS & University of Reading)
		. [The Errata system](https://github.com/NordicESMhub/nicest2-fair-hackathon/blob/main/content/presentations/errata_nicest2.pdf) (Atef Ben Nasser, IPSL/CNRS)
		- [ES-DOC tooling and internals](https://github.com/NordicESMhub/nicest2-fair-hackathon/blob/main/content/presentations/esdoc-2020-nicest2-cim2-cmip6.pdf) (Mark Greenslade IPSL/CNRS)
	- [DMP online](https://youtu.be/3GsvzOdLLWM) (Joakim Philipson, 75 mins.)

After the presentations, we had a general discussion to decide on the working groups for the hackathon itself. We had 3 working groups:
- **FAIR climate cookbook**: can we develop a guide for climate scientists to help them to make their data FAIR?
	- During our discussions, we tried to identify tools that are needed for capturing metadata. Some tools such as ESMValTool or Galaxy have already embedded provenance metadata and we should try to make sue of these tools as much as possible to improve the FAIRness of climate datae had interesting discussions on how to integrate DMPs and researchers workflows to ensure metadata is always propagated (automatically).
- **Reprohack**: reproduce scientific results detailed in a select published paper.
	- We selected the following paper: Humanitarian need drives multilateral disaster aid by Dellmuth, Lisa M. and Bender, Frida A.-M. and Jönsson, Aiden R. and Rosvold, Elisabeth L. and von Uexkull, Nina. PNAS January 26, 2021 118 (4) e2018293118; https://doi.org/10.1073/pnas.2018293118.
	- We had a lot of interesting discussions during our attempt to reproduce this paper. This is a very interesting exercise and we will publish the final report very soon where we provide feedback for publishers, data archive provider, Universities, libraries and research institutes, and of course the authors.
- **Ontogogies**: review existing ontologies used in the climate community.
	- Outcome of the discussion shows that there is a need for better coordination of the different existing initiatives.

### Identified bottlenecks for running efficiently NorESM and EC-Earth on euroHPC

Our first report on the identified bottlenecks for an efficient usage of Nordic ESMs on EuroHPC is now available!

We highlight below the most important findings:
- ESMs used in the Nordic countries are clearly not ready for EuroHPC and very little dedicated funding from the scientific community is used for porting existing codes to future architectures. Providers have hired several specialists to support the scientific community but the commitment from the scientific community is not there.
- Exchange of knowledge of involved staff (scientists, RSEs, technical support) would be very helpful. For instance, being able to organize meetings/hackathons (oneline or face to face) with both experts from NorESM and EC-EARTH has been highlighted as an important requirements by those involved in the GPU hackathon.
- Code refactoring and best software practices are the most important component for efficient usage of new architecture, including EuroHPC.


## Contribute to the NICEST2 Newsletter

- Do you organize an event or would like to share information on an upcoming event for the Earth System Modelling Community?
- Would you like to talk about your work on Earth System Modelling?

Please contact the NICEST2 project Manager (annefou-at-geo.uio.no).

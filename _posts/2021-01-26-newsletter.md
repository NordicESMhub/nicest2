---
layout: post
title: "NICEST2 newsletter"
subtitle: "26 January 2021"
date: 2021-02-04
background: '/img/posts/newsletter.png'
---

**Contributors**: *Jean Iaquinta*, *Anne Fouilloux*.

> ### Agenda
> {:.no_toc}
> 1. TOC
> {:toc}
>
{: .agenda}


Download [NICEST2 newsletter in PDF format](/nicest2/img/posts/2021-02-NICEST2Newsletter.pdf)


# Glossary for Nordic Climate

As part of the [NICEST2 project](https://neic.no/nicest2), we have started a list of definitions of commonly used [Climate Terms in the Nordic countries](https://nordicesmhub.github.io/nordic-climate-glossary/). 

The aim is also to include the list of Nordic institutions working on Climate in the Nordics and data repositories commonly used for these studies. 

See our [CONTRIBUTING guidelines](https://github.com/NordicESMhub/nordic-climate-glossary/blob/main/CONTRIBUTING.md) for adding your institutions, data repository, etc.

# Running NorESM with containers

Reproducing ESM simulations is particularly hard but container technology
can help to ensure exactly the same computing environment everywhere from your
laptop to the most powerful HPC.

[NorESM](https://github.com/NorESMhub/NorESM) can now be successfully run within a docker container:
- For more information check the [NorESM docker github repository](https://github.com/NorESMhub/NorESMCAM_docker).

Since October 2020, [Singularity is now available on HPCs from Sigma2](https://www.sigma2.no/experimental-support-singuarlity-containers-all-sigma2-systems)
(Saga, Fram and Betzy), and our next challenge will be to develop portable containers to carry out tests with multiple nodes and assess the performance of containerized applications 
compared to "bare metal" (ran directly on the host).

More information is available on our [NICEST2 Work Package 4 webpage](https://nordicesmhub.github.io/nicest2/2020/05/04/plan.html#wp4-esm-workflows-to-efficiently-run-noresm-and-ec-earth-on-eurohpc).

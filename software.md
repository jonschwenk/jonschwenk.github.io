---
layout: page
title: Software
permalink: /software/
---

I build and maintain research software that includes new algorithms, modeling frameworks, and reproducible pipelines. Some projects develop novel methods (RivGraph, VotE), some are end-to-end modeling efforts (e.g., DeepReservoir for RL-based reservoir operations and Pydro for differentiable runoff + routing); some are data-wranglers (dapper, satval, hillsloper). Across all of them, I turn messy, "big", multi-source environmental data into analysis-ready products and model-ready inputs. I’m big on reproducibility and automation—especially when it lets us ask new questions and see the world like we never have before.

I began coding during my PhD studies with Matlab, and later picked up Python when I started my postdoc. This is also when I found my passion for creating software through the development of RivGraph. Since then, I've branched into other languages and richer Python. Almost all of my packages have a geospatial component, and I frequently integrate Google Earth Engine. With the exception of `Pydro`, I was the primary developer for each package listed here, but many friends and collaborators have contributed ideas, knowledge, and code.

<div class="toc-pills">
  <a class="toc-pill" href="#deepreservoir">DeepReservoir</a>
  <a class="toc-pill" href="#pydro">Pydro</a>
  <a class="toc-pill" href="#vote">VotE (Veins of the Earth)</a>
  <a class="toc-pill" href="#dapper">dapper</a>
  <a class="toc-pill" href="#rivgraph">RivGraph</a>
  <a class="toc-pill" href="#rabpro">rabpro</a>
  <a class="toc-pill" href="#rivmap">RivMAP</a>
  <a class="toc-pill" href="#hillsloper">hillsloper</a>
  <a class="toc-pill" href="#satval">satval</a>
  <a class="toc-pill" href="#ecopopper">Ecopopper</a>
  <a class="toc-pill" href="#rivermuse">RiverMUSE</a>
</div>

---

<a id="deepreservoir"></a>
## DeepReservoir
<p style="margin-top:-1.3rem;"><em>(under development)</em></p>

DeepReservoir is a deep reinforcement learning framework for optimizing reservoir operations in a virtual hydropower-reservoir environment. It supports building scenario-driven environments (rules, constraints, objectives) and training policies with modern RL libraries, enabling rapid experimentation with alternative operational strategies.

- **Repository:** actively being developed; currently private. Contact me if interested.  
- **Tech:** deep reinforcement learning (stable-baselines3), simulation environments
- **Language(s):** Python

---

<a id="pydro"></a>
## Pydro 
<p style="margin-top:-1.3rem;"><em>(under development)</em></p>

Pydro is a differentiable runoff + routing modeling effort designed for hybrid physics/AI learning. The goal is to make hydrologic modeling components trainable end-to-end, while still retaining physically meaningful structure. Work to date includes development of a global wildfire–hydrology dataset (unreleased) for training and validation.

- **Repo:** email me  
- **Tech:** differentiable modeling
- **Language(s):** Python

---

<a id="vote"></a>
## VotE (Veins of the Earth)

<img
  src="{{ '/assets/images/software/vote/VotE.png' | relative_url }}"
  alt="VotE (Veins of the Earth) logo"
  loading="lazy"
  style="float:right; width:320px; max-width:45%; height:auto; margin:0 0 1rem 1rem;"
/>


It's hard to fully explain what VotE is. One on hand, it's just a database with a user-friendly API. On the other, it's a first-cut towards an ambitious vision to fuse global hydrologic data into a common, AI-ready platform that's in the direction of a "digital twin" (or "Hydrotwin" as I've pitched the idea a few times). It's given us a glimpse into the power of data fusion, the opportunities that still remain, and the ways it can let us re-imagine the questions we can ask about the Hydrosphere.

More concretely, VotE is a river-centric data platform and API for rapid querying, model building, and visualization across global river networks. It is designed around an AI-ready geospatial schema and workflows for integrating river-network–based datasets (e.g., hydrography, dams, attributes) into a consistent, queryable system for analysis and data-driven modeling.

The repository itself includes scripts to build VotE as well as the API (but not the data + database itself). It's somewhat messy; we are slowly bringing it toward something publicly releasable. Reach out if you're keen to see it!

- **Repo:** email me  
- **Tech:** PostgreSQL, PostGIS, geospatial data modeling, data fusion techniques
- **Pubs:** [Poster](https://www.authorea.com/doi/full/10.1002/essoar.10509913.2)
- **Language(s):** Python; SQL

---

<a id="dapper"></a>
<h2 class="software-logo-header" style="margin: 0.5rem 0 0.75rem 0;">
  <img src="{{ '/assets/images/software/dapper/dapper_logo_2.jpg' | relative_url }}"
       alt="dapper"
       loading="lazy"
       style="width:350px; max-width:100%; display:block;" />
</h2>

dapper (Data PreParation for ELM Runs) is a toolset for curating, sampling, and formatting the datasets needed to run DOE’s E3SM Land Model (ELM). It automates end-to-end data preparation workflows (meteorological forcings, parameters, and related inputs), leaning on Google Earth Engine and other APIs to make sampling fast, scalable, and flexible for different grid-cell definitions (e.g., polygons like watersheds rather than rectangular grids).

- **Repo:** https://github.com/lanl/dapper  
- **Tech:** Google Earth Engine (GEE), netCDF/xarray-style workflows, geospatial sampling
- **Language(s):** Python

---

<a id="rivgraph"></a>
<h2 class="software-logo-header" style="margin: 0.5rem 0 0.75rem 0;">
  <img src="{{ '/assets/images/software/rivgraph/rg_logo_full.png' | relative_url }}"
       alt="RivGraph"
       loading="lazy"
       style="height:100px; width:350px; max-width:100%; display:block;" />
</h2>

RivGraph is a Python package that extracts river and delta channel network topology (nodes/links) from georeferenced binary mask rasters. It automatically assigns link directionality and computes a range of topologic and morphologic network metrics, supporting reproducible studies of braided rivers and deltas.

- **Repo:** https://github.com/VeinsOfTheEarth/RivGraph  
- **Pubs:** [JOSS](https://doi.org/10.21105/joss.02952) · [ESurf Dynamics](https://www.earth-surf-dynam.net/8/87/2020/esurf-8-87-2020.html)
- **Tech:** image processing, graph analysis, geospatial I/O
- **Language(s):** Python

<div style="clear: both;"></div>

<figure style="clear: both; margin: 1.25rem auto; text-align: center;">
  <img
    src="{{ '/assets/images/software/rivgraph/rivgraph_directionality.png' | relative_url }}"
    alt="RivGraph example output"
    loading="lazy"
    style="display: block; margin: 0 auto; max-width: 900px; width: 95%; height: auto;"
  />
  <figcaption style="margin-top: 0.5rem;">
    <em>One of the novelties of RivGraph is that it can automatically set flow directions in its extracted channel networks.</em>
  </figcaption>
</figure>

---

<a id="rabpro"></a>
<h2 class="software-logo-header" style="margin: 0.5rem 0 0.75rem 0;">
  <img src="{{ '/assets/images/software/rabpro/rabpro_logo.png' | relative_url }}"
       alt="rabpro"
       loading="lazy"
       style="height:78px; width:250; max-width:100%; display:block;" />
</h2>

rabpro (River and Basin Profiler) delineates watershed basins and computes river profiles, slopes, and related longitudinal metrics at global scale. It can also compute contributing-basin statistics for arbitrary raster inputs (e.g., topography, precipitation, vegetation) via Google Earth Engine, providing a flexible bridge between user-defined locations and basin-scale context.

- **Repo:** https://github.com/VeinsOfTheEarth/rabpro  
- **Pubs:** [JOSS](https://doi.org/10.21105/joss.04237)
- **Tech:** Google Earth Engine (GEE), watershed delineation, raster statistics
- **Language(s):** Python

<figure style="clear: both; margin: 1.25rem auto; text-align: center;">
  <img
    src="{{ '/assets/images/software/rabpro/rabpro_workflow.png' | relative_url }}"
    alt="rabpro workflow"
    loading="lazy"
    style="display: block; margin: 0 auto; max-width: 900px; width: 95%; height: auto;"
  />
  <figcaption style="margin-top: 0.5rem;">
    <em>Among other things, rabpro automates zonal statistics using GEE's API.</em>
  </figcaption>
</figure>

---

<img
  src="{{ '/assets/images/software/rivmap/rivmap.png' | relative_url }}"
  alt="RivMAP functionality"
  loading="lazy"
  style="float:left; width:360px; max-width:45%; height:auto; margin:0 1.25rem 1rem 0;"
/>

RivMAP (River Morphodynamics from Analysis of Planforms) is a Matlab toolbox for extracting planform river morphodynamics from binary channel masks. It quantifies centerlines and banklines, width, migration rates, and cutoff events, and was built to support large-scale Landsat-based mapping of river planform change.

- **Repo:** [Mathworks](https://www.mathworks.com/matlabcentral/fileexchange/58264-rivmap-river-morphodynamics-from-analysis-of-planforms), [CSDMS](https://csdms.colorado.edu/wiki/Model:RivMAP)
- **Pubs:** [Earth and Space Science](https://doi.org/10.1002/2016EA000196)
- **Tech:** river planform analysis, image processing, Landsat workflows
- **Language(s):** Matlab

<div style="clear: both;"></div>

---

<a id="ecopopper"></a>
## Ecopopper

Ecopopper generates flexible, unstructured “ecopop units” to help bridge scale mismatches between Earth System Model grids and local ecological / population dynamics models. It supports coupling workflows and scenario experiments that need spatial units more meaningful than coarse model grid cells.

Ecopopper was part of a large LANL team's effort that resulted in two [R&D100 Awards](https://www.lanl.gov/media/news/0911-rd100-awards) in 2025.

- **Repo:** [GitHub](https://github.com/lanl/ecopop) 
- **Tech:** spatial clustering/typologies, scale-bridging units, ecology/hydrology
- **Language(s):** Python

<figure style="clear: both; margin: 1.25rem auto; text-align: center;">
  <img
    src="{{ '/assets/images/software/ecopop/ecopop_toronto.png' | relative_url }}"
    alt="rabpro workflow"
    loading="lazy"
    style="display: block; margin: 0 auto; max-width: 900px; width: 95%; height: auto;"
  />
  <figcaption style="margin-top: 0.5rem;">
    <em>Ecopop units were used to study mosquito-borne diseases over the Toronto Metro area (and continentally). These were designed to provide higher resolution over areas of either high human density or high mosquito habitat potential. (The first version of these units were called "Hydropop.").</em>
  </figcaption>
</figure>

---

<a id="rivermuse"></a>
## RiverMUSE

RiverMUSE simulates freshwater mussel population dynamics under changing suspended sediment and flow regimes, supporting scenario experiments that connect hydrology/sediment forcing to ecological response at reach scale. The model itself was a collaboration among coauthors; I merely coded it.

- **Repo:** [CSDMS](https://csdms.colorado.edu/wiki/Model:RiverMUSE) 
- **Pubs:** [Freshwater Science](https://www.journals.uchicago.edu/doi/full/10.1086/684223)
- **Tech:** ecohydrology, scenario simulation
- **Language(s):** Matlab

<figure style="clear: both; margin: 1.25rem auto; text-align: center;">
  <img
    src="{{ '/assets/images/software/rivermuse/rivermuse_model.png' | relative_url }}"
    alt="rivermuse model"
    loading="lazy"
    style="display: block; margin: 0 auto; max-width: 900px; width: 95%; height: auto;"
  />
  <figcaption style="margin-top: 0.5rem;">
    <em>A fairly simple interaction model resulted in rich dynamics, and its relative simplicity allowed for formal nonlinear dynamics analysis.</em>
  </figcaption>
</figure>

---

<a id="hillsloper"></a>
## hillsloper

hillsloper partitions DEMs into constituent hillslopes for high-resolution terrestrial simulations. It extracts a connected river network and maintains hillslope–channel connectivity, making it easier to build modeling domains that respect drainage structure and terrain controls.

- **Repo:** available upon request  
- **Tech:** DEM analysis, terrain partitioning, hydrologic connectivity
- **Language(s):** Python

<figure style="clear: both; margin: 1.25rem auto; text-align: center;">
  <img
    src="{{ '/assets/images/software/hillsloper/hillsloper.png' | relative_url }}"
    alt="Hillsloper example output"
    loading="lazy"
    style="display: block; margin: 0 auto; max-width: 900px; width: 95%; height: auto;"
  />
  <figcaption style="margin-top: 0.5rem;">
    <em>Hillsloper breaks DEMs into vector-based representations and characterizations amenable for use with ATS (Advanced Terrestrial Simulator)."</em>
  </figcaption>
</figure>


---

<a id="satval"></a>
## satval

satval samples multispectral satellite pixel features aligned in space and time with in-situ water-quality observations. It supports satellite–field validation and modeling by aggregating observations within shared pixel footprints and assembling analysis-ready matched datasets.

- **Repo:** available upon request  
- **Tech:** Google Earth Engine (GEE), remote sensing validation, water quality
- **Pubs:** [Journal of Applied Remote Sensing](https://www.spiedigitallibrary.org/journals/journal-of-applied-remote-sensing/volume-16/issue-4/044528/Geographically-aware-estimates-of-remotely-sensed-water-properties-for-Chesapeake/10.1117/1.JRS.16.044528.short)
- **Language(s):** Python

<figure style="clear: both; margin: 1.25rem auto; text-align: center;">
  <img
    src="{{ '/assets/images/software/satval/satval.png' | relative_url }}"
    alt="satval example output"
    loading="lazy"
    style="display: block; margin: 0 auto; max-width: 900px; width: 95%; height: auto;"
  />
  <figcaption style="margin-top: 0.5rem;">
    <em>Over 50 million water quality observations across the Chesapeake Bay were aligned in space/time with MODIS pixels to create a statistical model, all in "the cloud."</em>
  </figcaption>
</figure>

---


---
layout: software
title: Software
permalink: /software/
---

<div class="software-portfolio">
  <div class="software-intro">
    <p>I build research software that turns complex environmental data into usable models, methods, and analysis-ready products. The work ranges from new river-network algorithms and data platforms to end-to-end hydrologic modeling frameworks.</p>
    <p>Most projects are geospatial, reproducible, and automation-heavy. Except for Pydro, I have been the primary developer of each project shown here, with ideas, knowledge, and code contributed by many friends and collaborators.</p>
  </div>

  <section class="software-section" aria-labelledby="featured-software-heading">
    <h2 class="software-section__heading" id="featured-software-heading"><span>Featured software</span></h2>
    <p class="software-section__intro">Three projects that best represent the range of my current work: decision-making with AI, river-network algorithms, and global-scale data fusion.</p>

    <div class="software-feature-grid">
      <article class="software-feature software-feature--lead" id="deepreservoir">
        <div class="software-feature__media software-feature__media--deepreservoir" aria-hidden="true">
          <img src="{{ '/assets/images/index/human_impacts_banner2.png' | relative_url }}" alt="" />
          <span class="software-feature__eyebrow">Reservoir operations + reinforcement learning</span>
        </div>
        <div class="software-feature__content">
          <p class="software-status">In active development · Repository coming soon</p>
          <h3 id="deepreservoir-title">DeepReservoir-Navajo</h3>
          <p class="software-feature__summary">A deep reinforcement learning framework for optimizing reservoir operations in a virtual hydropower-reservoir environment. Scenario-driven rules, constraints, and objectives make it possible to test alternative operational strategies quickly.</p>
          <ul class="software-meta" aria-label="DeepReservoir-Navajo technologies">
            <li>Python</li>
            <li>stable-baselines3</li>
            <li>Simulation environments</li>
          </ul>
          <div class="software-links">
            <span class="software-link--pending" aria-label="GitHub repository coming soon">GitHub — coming soon</span>
            <a href="{{ '/contact/' | relative_url }}">Contact</a>
          </div>
        </div>
      </article>

      <article class="software-feature" id="rivgraph">
        <div class="software-feature__media software-feature__media--contain">
          <img src="{{ '/assets/images/software/rivgraph/rivgraph_directionality.png' | relative_url }}" alt="A river channel network with automatically assigned flow directions" loading="lazy" />
        </div>
        <div class="software-feature__content">
          <p class="software-status">Open source · Published</p>
          <h3 id="rivgraph-title">RivGraph</h3>
          <p class="software-feature__summary">Extracts river and delta channel-network topology from georeferenced masks, assigns link directionality, and computes reproducible topologic and morphologic metrics.</p>
          <ul class="software-meta" aria-label="RivGraph technologies">
            <li>Python</li>
            <li>Image processing</li>
            <li>Graph analysis</li>
          </ul>
          <div class="software-links">
            <a href="https://github.com/VeinsOfTheEarth/RivGraph">GitHub</a>
            <a href="https://doi.org/10.21105/joss.02952">JOSS</a>
            <a href="https://www.earth-surf-dynam.net/8/87/2020/esurf-8-87-2020.html">Methods paper</a>
          </div>
        </div>
      </article>

      <article class="software-feature" id="vote">
        <div class="software-feature__media software-feature__media--contain software-feature__media--vote">
          <img src="{{ '/assets/images/software/vote/VotE.png' | relative_url }}" alt="VotE, Veins of the Earth" loading="lazy" />
        </div>
        <div class="software-feature__content">
          <p class="software-status">Research platform · Source release planned</p>
          <h3 id="vote-title">VotE <span>(Veins of the Earth)</span></h3>
          <p class="software-feature__summary">A river-centric data platform and API for rapidly querying, modeling, and visualizing data across global river networks.</p>
          <ul class="software-meta" aria-label="VotE technologies">
            <li>Python + SQL</li>
            <li>PostgreSQL / PostGIS</li>
            <li>Geospatial data fusion</li>
          </ul>
          <div class="software-links">
            <a href="https://www.authorea.com/doi/full/10.1002/essoar.10509913.2">Poster</a>
            <a href="{{ '/contact/' | relative_url }}">Contact</a>
          </div>
          <details class="software-details software-details--feature">
            <summary>About VotE <svg viewBox="0 0 16 16" aria-hidden="true"><path d="M4 6l4 4 4-4" /></svg></summary>
            <div class="software-details__body">
              <p>VotE is a first step toward fusing global hydrologic data into a common, AI-ready platform—something in the direction of a hydrologic digital twin. Its schema and workflows bring hydrography, dams, and river attributes into one consistent, queryable system.</p>
              <p>The source currently includes build scripts and the API, but not the data or database. It is being prepared for a public release.</p>
            </div>
          </details>
        </div>
      </article>
    </div>
  </section>

  <section class="software-section software-section--more" aria-labelledby="more-software-heading">
    <h2 class="software-section__heading" id="more-software-heading"><span>More software</span></h2>
    <p class="software-section__intro">Focused tools and modeling efforts. Open a card for a workflow figure or additional context.</p>

    <div class="software-card-grid">
      <article class="software-card" id="rabpro">
        <div class="software-card__top">
          <div class="software-card__media software-card__media--wide-logo">
            <img src="{{ '/assets/images/software/rabpro/rabpro_logo.png' | relative_url }}" alt="rabpro, river and basin profiler" loading="lazy" />
          </div>
          <div class="software-card__copy">
            <p class="software-status">Open source · Published</p>
            <h3 id="rabpro-title">rabpro</h3>
            <p>Delineates watershed basins and computes river profiles, slopes, and contributing-basin statistics at global scale.</p>
            <ul class="software-meta" aria-label="rabpro technologies">
              <li>Python</li>
              <li>Google Earth Engine</li>
              <li>Raster statistics</li>
            </ul>
            <div class="software-links">
              <a href="https://github.com/VeinsOfTheEarth/rabpro">GitHub</a>
              <a href="https://doi.org/10.21105/joss.04237">JOSS</a>
            </div>
          </div>
        </div>
        <details class="software-details">
          <summary>Workflow example <svg viewBox="0 0 16 16" aria-hidden="true"><path d="M4 6l4 4 4-4" /></svg></summary>
          <div class="software-details__body">
            <p>rabpro connects user-defined locations to basin-scale context and can compute statistics for arbitrary raster inputs such as topography, precipitation, and vegetation through Google Earth Engine.</p>
            <figure>
              <img src="{{ '/assets/images/software/rabpro/rabpro_workflow.PNG' | relative_url }}" alt="rabpro basin delineation and zonal statistics workflow" loading="lazy" />
              <figcaption>rabpro automates basin delineation and zonal statistics using Google Earth Engine.</figcaption>
            </figure>
          </div>
        </details>
      </article>

      <article class="software-card" id="dapper">
        <div class="software-card__top">
          <div class="software-card__media software-card__media--wide-logo">
            <img src="{{ '/assets/images/software/dapper/dapper_logo_2.jpg' | relative_url }}" alt="dapper" loading="lazy" />
          </div>
          <div class="software-card__copy">
            <p class="software-status">Open source</p>
            <h3 id="dapper-title">dapper</h3>
            <p>Curates, samples, and formats the datasets needed to run DOE’s E3SM Land Model across flexible grid-cell definitions.</p>
            <ul class="software-meta" aria-label="dapper technologies">
              <li>Python</li>
              <li>Google Earth Engine</li>
              <li>netCDF / xarray</li>
            </ul>
            <div class="software-links">
              <a href="https://github.com/lanl/dapper">GitHub</a>
            </div>
          </div>
        </div>
        <details class="software-details">
          <summary>What it automates <svg viewBox="0 0 16 16" aria-hidden="true"><path d="M4 6l4 4 4-4" /></svg></summary>
          <div class="software-details__body">
            <p>dapper (Data PreParation for ELM Runs) automates meteorological forcings, parameters, and related inputs. It leans on Google Earth Engine and other APIs to make sampling scalable for polygons such as watersheds as well as rectangular grids.</p>
          </div>
        </details>
      </article>

      <article class="software-card" id="rivmap">
        <div class="software-card__top">
          <div class="software-card__media software-card__media--wide-logo">
            <img src="{{ '/assets/images/software/rivmap/rivmap_logo.png' | relative_url }}" alt="RivMAP, River Morphodynamics from Analysis of Planforms" loading="lazy" />
          </div>
          <div class="software-card__copy">
            <h3 class="visually-hidden" id="rivmap-title">RivMAP</h3>
            <p class="software-status">Open source · Published</p>
            <p>A Matlab toolbox for extracting planform river morphodynamics from binary channel masks, including widths, migration rates, and cutoff events.</p>
            <ul class="software-meta" aria-label="RivMAP technologies">
              <li>Matlab</li>
              <li>Image processing</li>
              <li>Landsat workflows</li>
            </ul>
            <div class="software-links">
              <a href="https://github.com/VeinsOfTheEarth/RivMAP">GitHub</a>
              <a href="https://doi.org/10.1002/2016EA000196">Paper</a>
            </div>
          </div>
        </div>
        <details class="software-details">
          <summary>Example outputs <svg viewBox="0 0 16 16" aria-hidden="true"><path d="M4 6l4 4 4-4" /></svg></summary>
          <div class="software-details__body">
            <figure>
              <img class="software-details__image--tall" src="{{ '/assets/images/software/rivmap/rivmap.PNG' | relative_url }}" alt="RivMAP centerline, bankline, width, migration, and cutoff outputs" loading="lazy" />
            </figure>
          </div>
        </details>
      </article>

      <article class="software-card" id="ecopopper">
        <div class="software-card__top">
          <div class="software-card__media software-card__media--figure">
            <img src="{{ '/assets/images/software/ecopop/ecopop_toronto.png' | relative_url }}" alt="Ecopop units around Toronto" loading="lazy" />
          </div>
          <div class="software-card__copy">
            <p class="software-status">Open source · R&amp;D 100–recognized team effort</p>
            <h3 id="ecopopper-title">Ecopopper</h3>
            <p>Generates flexible “ecopop units” that bridge scale mismatches between Earth System Model grids and local ecological or population models.</p>
            <ul class="software-meta" aria-label="Ecopopper technologies">
              <li>Python</li>
              <li>Spatial clustering</li>
              <li>Scale bridging</li>
            </ul>
            <div class="software-links">
              <a href="https://github.com/lanl/ecopop">GitHub</a>
              <a href="https://www.lanl.gov/media/news/0911-rd100-awards">Award</a>
            </div>
          </div>
        </div>
        <details class="software-details">
          <summary>Example application <svg viewBox="0 0 16 16" aria-hidden="true"><path d="M4 6l4 4 4-4" /></svg></summary>
          <div class="software-details__body">
            <p>The units shown for metropolitan Toronto provide higher resolution where either human density or mosquito-habitat potential is high. Ecopopper contributed to a larger LANL team effort that received two 2025 R&amp;D 100 Awards.</p>
          </div>
        </details>
      </article>

      <article class="software-card" id="pydro">
        <div class="software-card__top software-card__top--text">
          <div class="software-card__copy">
            <p class="software-status">In development · Available by request</p>
            <h3 id="pydro-title">Pydro</h3>
            <p>A differentiable runoff-and-routing modeling effort for hybrid physics/AI learning, designed to remain trainable end to end while retaining physically meaningful structure.</p>
            <ul class="software-meta" aria-label="Pydro technologies">
              <li>Python</li>
              <li>Differentiable modeling</li>
              <li>Hydrology</li>
            </ul>
            <div class="software-links">
              <a href="{{ '/contact/' | relative_url }}">Contact</a>
            </div>
          </div>
        </div>
        <details class="software-details">
          <summary>Current work <svg viewBox="0 0 16 16" aria-hidden="true"><path d="M4 6l4 4 4-4" /></svg></summary>
          <div class="software-details__body">
            <p>Work to date includes development of an unreleased global wildfire-hydrology dataset for training and validation.</p>
          </div>
        </details>
      </article>

      <article class="software-card" id="hillsloper">
        <div class="software-card__top">
          <div class="software-card__media software-card__media--figure">
            <img src="{{ '/assets/images/software/hillsloper/hillsloper.png' | relative_url }}" alt="Hillsloper terrain partition example" loading="lazy" />
          </div>
          <div class="software-card__copy">
            <p class="software-status">Available by request</p>
            <h3 id="hillsloper-title">hillsloper</h3>
            <p>Partitions digital elevation models into connected hillslopes for high-resolution terrestrial simulations while preserving hillslope-channel connectivity.</p>
            <ul class="software-meta" aria-label="hillsloper technologies">
              <li>Python</li>
              <li>DEM analysis</li>
              <li>Hydrologic connectivity</li>
            </ul>
            <div class="software-links">
              <a href="{{ '/contact/' | relative_url }}">Contact</a>
            </div>
          </div>
        </div>
        <details class="software-details">
          <summary>Modeling context <svg viewBox="0 0 16 16" aria-hidden="true"><path d="M4 6l4 4 4-4" /></svg></summary>
          <div class="software-details__body">
            <p>hillsloper creates vector-based terrain representations and characterizations suitable for the Advanced Terrestrial Simulator (ATS).</p>
          </div>
        </details>
      </article>

      <article class="software-card" id="satval">
        <div class="software-card__top">
          <div class="software-card__media software-card__media--figure">
            <img src="{{ '/assets/images/software/satval/satval.png' | relative_url }}" alt="Satellite and water-quality observation alignment" loading="lazy" />
          </div>
          <div class="software-card__copy">
            <p class="software-status">Available by request · Published</p>
            <h3 id="satval-title">satval</h3>
            <p>Matches multispectral satellite pixels with in-situ water-quality observations in space and time to build analysis-ready validation datasets.</p>
            <ul class="software-meta" aria-label="satval technologies">
              <li>Python</li>
              <li>Google Earth Engine</li>
              <li>Remote sensing</li>
            </ul>
            <div class="software-links">
              <a href="https://www.spiedigitallibrary.org/journals/journal-of-applied-remote-sensing/volume-16/issue-4/044528/Geographically-aware-estimates-of-remotely-sensed-water-properties-for-Chesapeake/10.1117/1.JRS.16.044528.short">Paper</a>
              <a href="{{ '/contact/' | relative_url }}">Contact</a>
            </div>
          </div>
        </div>
        <details class="software-details">
          <summary>Example application <svg viewBox="0 0 16 16" aria-hidden="true"><path d="M4 6l4 4 4-4" /></svg></summary>
          <div class="software-details__body">
            <p>More than 50 million Chesapeake Bay water-quality observations were aligned in space and time with MODIS pixels in the cloud to create a statistical model.</p>
          </div>
        </details>
      </article>

      <article class="software-card" id="rivermuse">
        <div class="software-card__top">
          <div class="software-card__media software-card__media--figure">
            <img src="{{ '/assets/images/software/rivermuse/rivermuse_model.PNG' | relative_url }}" alt="RiverMUSE population-dynamics model" loading="lazy" />
          </div>
          <div class="software-card__copy">
            <p class="software-status">Model available · Published</p>
            <h3 id="rivermuse-title">RiverMUSE</h3>
            <p>Simulates freshwater mussel population dynamics under changing suspended-sediment and flow regimes at reach scale.</p>
            <ul class="software-meta" aria-label="RiverMUSE technologies">
              <li>Matlab</li>
              <li>Ecohydrology</li>
              <li>Scenario simulation</li>
            </ul>
            <div class="software-links">
              <a href="https://csdms.colorado.edu/wiki/Model:RiverMUSE">CSDMS</a>
              <a href="https://www.journals.uchicago.edu/doi/full/10.1086/684223">Paper</a>
            </div>
          </div>
        </div>
        <details class="software-details">
          <summary>Model context <svg viewBox="0 0 16 16" aria-hidden="true"><path d="M4 6l4 4 4-4" /></svg></summary>
          <div class="software-details__body">
            <p>The model was a collaboration among coauthors; I implemented it in code. A relatively simple interaction model produced rich dynamics and remained tractable for formal nonlinear-dynamics analysis.</p>
          </div>
        </details>
      </article>
    </div>
  </section>
</div>

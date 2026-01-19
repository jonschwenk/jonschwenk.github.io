---
layout: page
title: Research
permalink: /research/
---

I work at the intersection of hydrology, Earth observation, and AI to improve environmental understanding and decision support. I aim to create *usable* science: methods and open tooling that can turn large, messy, multi-source datasets into analysis-ready products and model-ready inputs. I am also interested in fundamental (and sometimes esoteric) ideas, but have lately struggled to pursue research that doesn't have a pathway toward meaningful impact.

<div class="toc-pills">
  <a class="toc-pill" href="#data-fusion">Hydrotwin</a>
  <a class="toc-pill" href="#rivers">Rivers & deltas</a>
  <a class="toc-pill" href="#decisions">Predictions to decisions</a>
  <a class="toc-pill" href="#river-extraction">Watching from space</a>

</div>

---

<a id="data-fusion"></a>
## Hydrotwin

**Overarching question:** *How can we fuse disparate hydrologic observations into a coherent, living, AI-ready view of the hydrosphere?*

Modern hydrology is data-rich, but the data are fragmented: different formats, spatial supports, identifiers, and implicit assumptions. My aim is to reduce the cost of asking (and answering) interesting scientific questions by building platforms that make heterogeneous observations easier to discover, combine, and learn from. We are rapidly approaching the point where *digital twinning* of the hydrosphere (Hydrotwin) is becoming more realistic through smart fusion of satellite and in-situ data globally.

- **VotE**: a *Hydrotwin* prototype; a river-centric data platform and API designed around an AI-ready geospatial schema.
- Focus areas include schema design for network-based geospatial data, reproducible build workflows, database design and management, and intuitive query/analysis interfaces.

**For more information:**
- Software: [VotE (Veins of the Earth)](/software/#vote)
- Publications: [VotE AGU Poster](https://www.authorea.com/doi/full/10.1002/essoar.10509913.2) · [GRIT](https://doi.org/10.1029/2024WR038308)

---

<a id="decisions"></a>
## Predictions to decisions

**Overarching question:** *How do we connect prediction to real-world management in water systems?*

Prediction is only valuable if it can be translated into decisions under constraints. I’m interested in the tools (and scientific framing) that make that translation possible—especially when uncertainty, competing objectives, and changing conditions matter. I also explore the use of AI for forecasting hydrologic variables relevant to decisionmaking.

- **DeepReservoir**: a deep reinforcement learning framework for optimizing reservoir operations in simulated hydropower-reservoir environments.
- Closely related interests include hybrid physics + ML modeling and differentiable modeling components (see also [Pydro](/software/#pydro)).

**For more information:**
- Software: [DeepReservoir](/software/#deepreservoir)
- Publications: [Streamflow](https://doi.org/10.1029/2024EA003798) · [Stream temperature](https://doi.org/10.1029/2024WR039053) · [Water quality](https://doi.org/10.1117/1.JRS.16.044528) · [River ice breakup](https://doi.org/10.1029/2025WR040635)

---

<a id="rivers"></a>
## Rivers & deltas

**Overarching question:** *How do rivers and deltas organize themselves graphically, and what can we learn from imagery at scale?*

River planform patterns record physics, ecology, and human influence. A big chunk of my early work focused on turning satellite-derived masks into representations that are amenable to measurement, statistics, and learning.

- **RivGraph**: extracts river/delta channel networks from imagery and represents them as graphs (nodes/links).
- Enables reproducible network measurements (topologic + morphologic metrics) and supports learning on graph-structured representations.
- **RivMAP**: quantifies how river patterns change across time over large spatial domains.

**For more information:**
- Software: [RivGraph](/software/#rivgraph) · [RivMAP](/software/#rivmap)
- Publications: [RivMAP](https://doi.org/10.1002/2016EA000196) · [RivGraph](https://doi.org/10.21105/joss.02952) · [Flow directions](https://www.earth-surf-dynam.net/8/87/2020/esurf-8-87-2020.html) · [Permafrost and bank erosion](https://doi.org/10.1029/2023JF007101) · [Nitrate in deltas](https://doi.org/10.1029/2022GL102201)

---

<a id="river-extraction"></a>
## Watching from space

**Overarching question:** *How can we identify and map rivers from satellite imagery in an automated, scalable way—without losing the connectivity and geometry that make rivers “rivers”?*

Satellite archives contain the information needed to "watch" rivers at a global scale. The hard part is developing reliable, scalable automated algorithms that transform satellite reflectances into river masks (binary images of river presence) that can be measured. Pixel-wise segmentation can produce decent masks, but it often struggles with the features that matter most for hydrology and geomorphology: connected networks, branching structure, centerlines, and consistent topology across space and time. I have used various ML/AI methods to attack this problem, but have yet to find a silver bullet. My most recent attempt was work with PhD student Bohan Chen (UCLA) to use graph-based learning--the approach showed promise (similar accuracies to DeepWaterMap with orders-of-magnitude fewer training samples).

This line of work is closely aligned with my broader interest in **turning remote sensing into analysis-ready and model-ready products**, and it connects naturally to graph-based representations and tooling (e.g., RivGraph) where networks become measurable, learnable objects rather than static masks.

**For more information:**
- Publications: [Graph learning](https://doi.org/10.1109/IGARSS52108.2023.10282009) · [Graph learning improved](https://doi.org/10.1007/s42967-023-00284-8) · [Graph learning pipeline](https://doi.org/10.1109/JSTARS.2024.3493073) 


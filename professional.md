---
layout: page
title: Work
permalink: /professional/
lede: Ten years of distributed systems and scientific computing, from LHC analysis at CERN to machine learning on petabyte-scale satellite data for carbon monitoring.
---

## Chloris Geospatial

<div class="role-head"><h3>Head of Engineering</h3><span>May 2022 – present · Boston</span></div>
<p class="role-title">Data Engineer → Senior Software Engineer → Principal Engineer → Head of Engineering</p>

[Chloris](https://chloris.earth) measures forest carbon from satellite imagery. I joined as one of two engineers and now lead the engineering team.

- Built a petabyte-scale geospatial data platform whose Dask workloads, on thousands of AWS workers, produce Chloris's commercial product: global carbon-stock maps spanning 25 years.
- Engineered the production ML pipeline behind those maps, from satellite feature generation through model training to continental-scale distributed inference.
- Designed the engine behind Chloris's customer-facing carbon statistics for 72 countries. It aggregates arbitrary regions across the global Sentinel-2 grid (about 20,000 tiles in differing projections) without reprojecting pixels.
- Made spatially correlated confidence intervals on carbon aggregates tractable at continental scale, by approximating an O(N²) error-covariance sum over hundreds of millions of pixels with a banded stencil.
- Now re-architecting the pipeline: Dagster-orchestrated builds of sharded Zarr cubes, GPU inference for PyTorch models on optical and radar time series, and versioned products in a STAC catalog.

## Particle physics at UCLA and CERN

<div class="role-head"><h3>PhD candidate, then postdoctoral researcher</h3><span>2016 – 2022 · Los Angeles and Geneva</span></div>

My [thesis](https://escholarship.org/uc/item/3gw9h84p) analyzed collisions in the Compact Muon Solenoid (CMS) detector at the Large Hadron Collider. Protons collide 40 million times a second, far too often to record every event: particles from one collision are still on their way out of the detector when the next one happens. A chain of fast triggers decides, in real time, which collisions are worth keeping. The UCLA group specializes in muons, whose clean signature makes them good for this.

**A sharper muon trigger.** I designed a C++ pattern-recognition algorithm that doubles the position resolution of the low-level hits used to reconstruct muons, so the trigger can better tell an interesting collision from a common one. Its lookup tables were deployed to the detector's FPGA firmware at no added latency, and run in LHC Run 3.

**A search for long-lived particles.** I searched for a neutral particle that travels some distance before decaying into two muons, a possible dark-matter signature. The analysis used the whole detector, with custom reconstruction and data-driven background estimates written in C++ and distributed Python on the CERN grid, to narrow hundreds of quadrillions of collisions to a few tens of candidates. The resulting limits were world-leading ([JHEP 05 (2023) 228](https://link.springer.com/article/10.1007/JHEP05(2023)228)).

## Mevion Medical Systems

<div class="role-head"><h3>Software Engineer, Physics and Algorithms</h3><span>2014 – 2016 · Littleton, MA</span></div>

- Developed real-time algorithms that modulate proton-beam position on a 250 MeV synchrocyclotron used for cancer treatment.
- Built a GEANT4 particle-transport simulation farm on AWS for radiation-field modeling and verification.
- Simulated and tested a water-cooled, dual-axis magnet prototype.

## Education, awards and papers

Education
: PhD in Physics, UCLA, 2022
: MS in Physics, UCLA, 2017
: BA in Physics, Boston University, 2014, *cum laude*

Awards
: [Breakthrough Prize in Fundamental Physics](https://breakthroughprize.org/), 2025, awarded to the LHC collaborations (as a CMS member)
: AWS Certified Machine Learning – Specialty, 2023
: [CERN EcoActions](https://eco-actions.web.cern.ch/) Hackathon, 2021, second place

Papers
: CMS Collaboration, "Search for long-lived particles decaying to a pair of muons in pp collisions at √s = 13 TeV", [JHEP 05 (2023) 228](https://link.springer.com/article/10.1007/JHEP05(2023)228)
: [CMS author](https://cds.cern.ch/collection/CMS%20Papers) since 2019
: W. Nash, C. Grefe, "Beam Profiling through Wire Chamber Tracking", [LCD-Note-2013-009](https://cds.cern.ch/record/1571199/files/LCD-Note-2013-009-final.pdf), 2013

Notes
: [Comprehensive exam notes]({{ '/assets/comp-notes.pdf' | relative_url }}): roughly everything a physics undergraduate should know, written while studying for UCLA's [doctoral exam]({{ '/assets/comp-exam.pdf' | relative_url }})
: [Profiling nuisance parameters]({{ '/assets/profile-likelihood.pdf' | relative_url }}): an exact solution for the multinomial likelihood, from a statistics course project

Outreach
: CERN Open Days, 2019
: UCLA [Exploring Your Universe](https://www.exploringyouruniverse.org/), 2017 and 2018

## Tools

Languages
: Python, C++, JavaScript, shell

Data and ML
: PyTorch, LightGBM, scikit-learn, Dask, Dagster, NumPy, pandas, Numba, Xarray, Zarr, GDAL, STAC

Infrastructure
: AWS, Kubernetes, Docker, Terraform, GitLab CI, SQL

Physics
: ROOT, GEANT4, HTCondor, Monte Carlo methods

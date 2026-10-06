---
layout: page
title: Work
permalink: /professional/
lede: Ten years of distributed systems and scientific computing, from the Large Hadron Collider to climate.
---

<p class="label">Experience</p>
<ul class="rows">
  <li class="row">
    <span class="when">2022 – now</span>
    <div><strong>Head of Engineering</strong> <span class="org">· Chloris Geospatial, Boston</span>
      <p><a href="https://chloris.earth">Chloris</a> measures forest carbon from satellite imagery. I joined as one of two engineers and now lead the engineering team.</p>
      <ul>
        <li>Built a petabyte-scale geospatial data platform whose Dask workloads, on thousands of AWS workers, produce Chloris's commercial product: global carbon-stock maps spanning 25 years.</li>
        <li>Engineered the production ML pipeline behind those maps, from satellite feature generation through model training to continental-scale distributed inference.</li>
        <li>Designed the engine behind Chloris's customer-facing carbon statistics for 72 countries. It aggregates arbitrary regions across the global Sentinel-2 grid (about 20,000 tiles in differing projections) without reprojecting pixels.</li>
        <li>Made spatially correlated confidence intervals on carbon aggregates tractable at continental scale, by approximating an O(N²) error-covariance sum over hundreds of millions of pixels with a banded stencil.</li>
        <li>Now re-architecting the pipeline: Dagster-orchestrated builds of sharded Zarr cubes, GPU inference for PyTorch models on optical and radar time series, and versioned products in a STAC catalog.</li>
      </ul>
    </div>
  </li>
  <li class="row">
    <span class="when">2016 – 2022</span>
    <div><strong>PhD candidate, then postdoc</strong> <span class="org">· UCLA and CERN</span>
      <p>My <a href="https://escholarship.org/uc/item/3gw9h84p">thesis</a> analyzed collisions in the Compact Muon Solenoid (CMS) detector at the Large Hadron Collider. Protons collide 40 million times a second, far too often to record every event: particles from one collision are still leaving the detector when the next one happens. A chain of fast triggers decides, in real time, which collisions are worth keeping.</p>
      <p><em>A sharper muon trigger.</em> I designed a C++ pattern-recognition algorithm that doubles the position resolution of the low-level hits used to reconstruct muons, so the trigger can better tell an interesting collision from a common one. Its lookup tables were deployed to the detector's FPGA firmware at no added latency, and run in LHC Run 3.</p>
      <p><em>A search for long-lived particles.</em> I searched for a neutral particle that travels some distance before decaying into two muons, a possible dark-matter signature. Custom reconstruction and data-driven background estimates, written in C++ and distributed Python on the CERN grid, narrowed hundreds of quadrillions of collisions to a few tens of candidates. The resulting limits were world-leading (<a href="https://link.springer.com/article/10.1007/JHEP05(2023)228">JHEP 05 (2023) 228</a>).</p>
    </div>
  </li>
  <li class="row">
    <span class="when">2014 – 2016</span>
    <div><strong>Software Engineer, Physics and Algorithms</strong> <span class="org">· Mevion Medical Systems, Littleton, MA</span>
      <ul>
        <li>Developed real-time algorithms that modulate proton-beam position on a 250 MeV synchrocyclotron used for cancer treatment.</li>
        <li>Built a GEANT4 particle-transport simulation farm on AWS for radiation-field modeling and verification.</li>
        <li>Simulated and tested a water-cooled, dual-axis magnet prototype.</li>
      </ul>
    </div>
  </li>
</ul>

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

---
layout: page
title: Professional
---

I just finished my [PhD in Experimental Particle Physics](https://escholarship.org/uc/item/3gw9h84p) at UCLA. I have experience as a software engineer before attending graduate school and know my way around data analysis, statistics, algorithms, control systems and particle physics. Having spent years studying the arcane world of particle physics, I hope to move into a field where clever ideas are needed to solve problems that have a real impact on our future. A condensed version of my resume can be found in the sidebar with more details contained below

- [Physics](#physics)
- [Statistics](#statistics)
- [Software](#software)
- [Miscellaneous](#miscellaneous)

<a name="physics"></a>
## Physics

My thesis work involves analysis of collisions within the Compact Muon Solenoid (CMS) detector at the Large Hadron Collider. Within CMS, every so-called "event" cannot be recorded to disk due to bandwidth limitations associated with the high 40 MHz collision frequency. To illustrate this point, particles produced by a collision leaving the detector at the speed of light are only part way out of the detector when the next collision takes place. This rapid succession of collisions therefore requires a series of low-level triggers to select events with particles which are worth recording. In particular, the UCLA CMS group has expertise with muons which have an experimental signature not easily confused with others particles, therefore making them useful for investigating the underlying event.

For the first part of my thesis, I developed and verified an algorithm that improves the position resolution of low-level primitives used in reconstructing muons by a factor of two. This translates into a trigger that can more easily discern an interesting event from a more common, less interesting one. The algorithm was implemented and tested with a simulation of the reconstruction firmware I wrote in C++, which feeds the individual detector hits into a lookup table.

For the second part of my thesis, I conducted a search for a long-lived neutral particle which decays into two muons. This analysis uses the full extent of the CMS detector to look for potential dark matter candidates which could be produced using the 13 TeV center of mass energy of each collision. Data recorded at CMS is analyzed and then piped through a series of selection criteria to select for well measured candidate events. Our analysis selects only a few tens of candidates down from the hundreds of quadrillions of initial collisions. Expected 95% confidence level upper-limits on the production cross-section are then calculated using a likelihood function combining the expected number background events and various systematic uncertainties. 

Academic
: 2014 - BA in Physics from Boston University *cum laude*
: 2017 - MS in Physics from UCLA
: 2022 - PhD in Physics from UCLA

Publications
: [CMS Author][cms-author]: Feb 24, 2019 - Present
: W.Nash, C.Grefe, “*Beam Profiling through Wire Chamber Tracking*”, [LCD-Note-2013-009][beam-profiling], 2013

<!-- Teaching
: I have taught... -->

Comprehensive Exam
: Physics doctoral students must pass a comprehensive [exam][exam] at UCLA in order to continue their studies. I wrote [these notes][notes] while studying, which cover roughly all the material an undergraduate should know at the end of their Bachelor's degree.

<a name="statistics"></a>
## Statistics

<!-- My research involves ... -->


Profile Likelihood
: My statistics course [final project][likelihood] covers an exact solution I had derived to profile nuisance parameters for the multinomial distribution
<!-- : The general idea is that if the Likelihood function is dependent on many variables, you can "profile" out the variables you don't need (called nuisance parameters). -->

<a name="software"></a>
## Software

<!-- Implemented gitlab CI and code testing -->

Languages
: `python`, `C++`, `bash`, `Markdown`, `LaTeX`, `CSS`

Programs
: [`awkward`][awkward], [`coffea`][coffea], `numpy`, `git`, `matplotlib`, [`ROOT`][root], `pandas`, `scipy`, `numba`, `tensorflow`, `Qt`, `gimp`

Slides
: My [talk template][talk] was designed with [remark][remark]
: See the source code [here][talk-source]

Website
: I modified the [Hyde][hyde] template from [Mark Otto][otto] and host it using GitHub [pages][pages]


<a name="miscellaneous"></a>
## Miscellaneous

Awards
: [CERN EcoActions][cern-eco-actions] Hackathon 2021: Second Place

Volunteering
: [CERN Open Days 2019][open-days]
: [UCLA Explore Your Universe 2018][eyu]
: [UCLA Explore Your Universe 2017][eyu]


Fraternity
: Sigma Alpha Mu Scholarship Chair 2011-2013



[beam-profiling]: https://cds.cern.ch/record/1571199/files/LCD-Note-2013-009-final.pdf
[cms-author]: https://cds.cern.ch/collection/CMS%20Papers
[notes]: /assets/comp-notes.pdf
[exam]: /assets/comp-exam.pdf

[likelihood]: /assets/profile-likelihood.pdf

[awkward]: https://awkward-array.org/quickstart.html
[coffea]: hhttps://coffeateam.github.io/coffea/index.html
[root]: https://root.cern.ch/
[talk]: https://williamnash.github.io/talk-template/
[remark]: https://github.com/gnab/remark
[talk-source]: https://github.com/williamnash/talk-template
[hyde]: https://hyde.getpoole.com/about/
[otto]: https://twitter.com/mdo
[pages]: https://pages.github.com/

[cern-eco-actions]: https://eco-actions.web.cern.ch/
[open-days]: https://opendays.cern/
[eyu]: https://www.exploringyouruniverse.org/

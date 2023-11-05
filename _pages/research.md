---
title: "My Research"
permalink: /research/
author_profile: true
redirect_from:
  - /resume
---

... focuses on **high-energy astrophysics**, in particular **non-thermal particle acceleration** in **fast outflows** and the subsequent energy dissipation ("**radiation modeling**") into **multi-messenger signatures**, including **cosmic rays, photons and neutrinos**. I have experience with two promising candidate sites: **relativistic shocks in gamma-ray burst (GRB) afterglows** and **magnetic reconnection in blazar jets**.

I believe that the **combination of observations** (in particular their limitations) **and theory** (analytical and numerical modeling) provides the best environment for progress in understanding.

## Gamma-ray burst (GRB) afterglows

### Flat energy spectra up to the highest energies - Lepto-hadronic scenarios
Motivated by the emerging observational picture that GRB afterglows with detection up to TeV energies show relatively hard spectra ($ \mathrm{d} \ln N_\gamma/\mathrm{d} \ln E_\gamma \sim -2$), we are investigating scenarios how to extend the spectrum using the radiative signatures of the protons likely to be accelerated in the relativistic shock too. Besides the leptonic scenarios like the SSC scenario and the one with the extended synchrotron-component, we also explore scenarios like the proton-synchrotron, a combination of electron and synchrotron components, and scenarios involving the hadronic cascade initiated by the proton-proton interactions in a denser environment like a molecular cloud. To study this I coupled a numerical model for the dynamics of the blast wave to the timedependent, numerical one-zone solver [AM³](https://gitlab.desy.de/am3/am3). Below you see a preliminary result for the proton-synchrotron scenario. The paper is in preparation - stay tuned!

![Proton-Synchrotron-Model](/files/research_images/GRB_AG_psynmodel.png)

--- 

### Counts-level fits to GRB 221009A - [arXiv:2308.13854](https://arxiv.org/abs/2308.13854)
By far the brightest GRB detected so far - and behind the Galactic plane. This combination leads to a challenging observational situation for our data from *Swift*-XRT and *Fermi*-LAT. For *Swift*-XRT the dust rings around the source hinder our background estimation significantly, while the background estimate with *Fermi*-LAT's background templates and the limited statistics is limiting our inference of the spectrum up to energies higher than a few GeV. Taking into account the effects, and correcting where possible, we combine the data with the one from *Swift*-BAT during two contemporaneous time windows at $T_{0,\mathrm{GBM}}+4~\mathrm{ks}$ and $T_{0,\mathrm{GBM}}+22~\mathrm{ks}$ and perform a combined fit at the counts level (using [3ML](https://threeml.readthedocs.io/en/stable/index.html)) to a synchrotron model (see below). We find that the spectrum is described well by a power-law from $10~\mathrm{keV} - 10~\mathrm{GeV}$, with a photon spectral index of about 2.2 (similar to earlier LHAASO observations). Below $10~\mathrm{keV}$ we find a break that can be interpreted in 3 scenarios: Fast cooling, slow cooling or their transition. See the paper for more details!

![Fit to GRB221009A's early afterglow](/files/research_images/GRB221009A_Afterglow_fit.png)

---

### Counts-level fits to GRB 190114C -[arXiv:2206.11148](https://arxiv.org/abs/2206.11148)

After the detection of GRB 190114C with the MAGIC telescopes at TeV energies an ongoing debate about the origin of this radiation has started. The contemporaneous *Fermi*-LAT data (5 and 6 photons) visually suggested a slightly lower flux compared to the measurements at lower energies, which was interpreted as a confirmation of the two-component synchrotron self-Compton (SSC) model. In order to answer the question of preference for a new component, we compared the SSC model at the counts-level (using [3ML](https://threeml.readthedocs.io/en/stable/index.html)) to a single-component model with only one extendend synchrotron component. We find no preference from the data for either of the two models - and no relevance of the *Fermi*-LAT data. See below the envelopes of the two models - you also hardly see any difference by eye!

![GRB190114C best fit SEDs](/files/research_images/GRB190114C_SED_comparison.png)

---

## Radiation modeling with [AM³](https://gitlab.desy.de/am3/am3)

Started already earlier within the [NEUCOS](https://www-zeuthen.desy.de/~wwinter/) project at DESY Zeuthen, we are currently in the final phase of making the radiation modeling code AM³ (Astrophysical Multi-Messenger Modeling) public. It solves the coupled transport equations for for protons, electrons, photons, pions, muons and neutrinos and has all the relevant radiaton processes/interactions (Syn, IC, pair-prod., p𝛾, pp, Bethe-Heitler, decays,...) implemented. Two particular features are its speed optimisation options and the tracking of all the different components in the particle spectra. It is originally written in C++, but has a convenient interface to python. Stay tuned for the public version!

---


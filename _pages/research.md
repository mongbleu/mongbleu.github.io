---
layout: single
permalink: /research/
title: "Research"
author_profile: true
toc: true
toc_label: "Research threads"
---

Three threads, one question: **how much of a physical model should survive inside a learned one, and what does the surviving structure buy you when the data thins out?**

## Knowledge-guided AI for environmental decision support {#knowledge-guided-ai}

Environmental decisions are made exactly where observations are thinnest — a county with no flux tower, a forest with no inventory plot, a basin with three gauges. Pure data-driven models extrapolate badly there; pure process models are too rigid to absorb what data does exist. My work sits on the seam.

**Differentiable process models.** In the wildfire work, I reformulated a Rothermel-type fire-spread model as a differentiable CNN layer, so gradients flow through the physics. The physical structure constrains learning where burned-area observations are sparse, instead of the network inventing its own dynamics.
→ [Crown base height model](/models/crown-base-height/) · manuscript under review at *Ecological Informatics* · patent KR 10-2025-0189148

**Allometry as an inductive bias.** Crown base height across 36 tree species is not learnable from plot data alone. Embedding allometric forest structure relationships into the model keeps predictions physically ordered — crown base below crown top, monotone in stand density — in species with a handful of observations.
→ [Trained model, maps, and training data on Zenodo](https://doi.org/10.5281/zenodo.21736584)

**Domain adaptation across regions.** Land-cover classification transfers poorly into regions without ground truth. A phenological classification framework let a model trained in the South be applied to North Korea.
→ Kim et al. (2024), *Ecological Informatics* — [DOI](https://doi.org/10.1016/j.ecoinf.2024.102576)

**Open question I want to work on:** when the process model and the learned residual disagree, current practice picks one by validation score. Is there a principled decomposition — and can the disagreement itself be used as a diagnostic of missing process?

## Behavioral modeling and reinforcement learning {#behavioral-modeling}

Hydrological models treat human water use as a boundary condition. It is not — it is a decision, made repeatedly, under uncertainty, by agents who learn.

**SWAT–ABM coupling at basin scale.** I coupled a process-based hydrological model (SWAT) with an NSGA-II behavioral model, simulating roughly one million farming households in the Yeongsan River Basin under climate and management scenarios, to assess food–water–biodiversity trade-offs.
→ [Model details](/models/swat-abm-nexus/) · EGU 2025 (oral), EGU 2023 (oral) · manuscript in preparation

**Where I want to take it.** NSGA-II agents optimize a fixed objective; they do not *learn*. The direction I am preparing for doctoral work replaces the optimization core with reinforcement learning, coupled to a hydrology–agriculture simulator in the spirit of the GEB framework — agents that adapt their strategy as the basin changes, and that can be interrogated for what policy actually shifted behavior.

**Open question I want to work on:** an RL agent that reproduces observed cropping decisions is not the same as one that responds correctly to an unseen policy. What validation protocol separates the two?

## Satellite-based monitoring of land–carbon dynamics {#land-carbon}

Carbon neutrality is legislated nationally and implemented locally. The spatial resolution of the evidence has to match the scale of the decision.

**Local-scale carbon balance.** I built an AI-driven spatial model predicting greenhouse gas emissions at 1-hectare resolution, and a carbon balance typology that classifies Korean local governments by the structure of their sources and sinks — so a municipality can see which lever is actually available to it.
→ [Model and code](/models/carbon-balance/) · *J. Climate Change Research* (2024) · M.S. thesis, Korea University

**National inventories from imagery.** U-Net land cover mapping for the national GHG inventory of Korean ecosystem types, and aerial image analysis for the LULUCF Settlement sector inventory.

**Field-scale application.** For UN ESCAP, I designed a carbon neutral village model for rural Nepal and estimated mitigation and adaptation outcomes from field-collected data — the same accounting logic, at the smallest unit where people actually act.
→ [UN ESCAP report (2025)](https://hdl.handle.net/20.500.12870/8214)

**Open question I want to work on:** downscaled emission maps are validated against the aggregate they were downscaled from. That is circular. What independent observation constrains a 1-hectare emission estimate?

---

Currently I also design the analytical framework behind the [Climate Technology Cooperation Strategy Map](/models/climate-tech-strategy-map/) at NIGT — a deployed platform that turns technology, capacity, and needs data into a partner-selection decision for international climate cooperation.

---
permalink: /
title: "Yujeong Jeong"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

I build **hybrid environmental models that put physical process knowledge inside machine learning**, so that climate and land decisions can be made where observations are sparse and where the decision is actually taken — a watershed, a municipality, a village.

I am a post-master researcher at the **National Institute of Green Technology (NIGT)**, Republic of Korea, working on climate technology cooperation strategy for developing countries. Before that, at Korea University's Environmental GIS/RS Lab and the OJeong Resilience Institute, I converted a physics-based fire-spread model into a differentiable CNN layer to learn under sparse observations, coupled a process-based hydrological model with a behavioral agent-based model over one million farming households, and built a 1-hectare-resolution carbon balance model now used to type every local government in Korea.

Every model I build is released — as code, as a trained model with a DOI, or as a deployed platform. **[Models & Data](/models/)** is the part of this site I keep most current; the papers are downstream of what is there.

The question underneath all of it: **when a process-based model and a data-driven model disagree, what is the principled way to let them correct each other — and does the resulting model actually change what a decision-maker does?** I am preparing doctoral research that pushes this toward reinforcement-learning-based agent behavior coupled with a hydrology–agriculture simulator (SWAT–ABM, in the direction of the GEB framework), where agents *learn* rather than optimize a fixed objective.

## What I work on

**[Knowledge-guided AI for environmental decision support](/research/#knowledge-guided-ai)** — differentiable and hybrid modeling that embeds physical or allometric structure into neural networks, so models stay physically sensible where data runs out.

**[Behavioral modeling and reinforcement learning](/research/#behavioral-modeling)** — agent-based simulation of land and water use decisions under climate and policy scenarios, at the scale of a full river basin.

**[Satellite-based monitoring of land–carbon dynamics](/research/#land-carbon)** — U-Net land cover mapping, national GHG inventories, and local-scale carbon balance at 1-hectare resolution.

## Models, data, and platforms

| | What it is | Access |
|---|---|---|
| **Hybrid crown base height model** | Allometric structure embedded in ML; 36 tree species; input to a crown fire simulation module | [Zenodo DOI](https://doi.org/10.5281/zenodo.21736584) · patent pending · [details](/models/crown-base-height/) |
| **Local-scale carbon balance model** | 1-ha resolution GHG emission model and carbon-neutrality typology for Korean local governments | [GitHub](https://github.com/mongbleu/carbonBalance) · [details](/models/carbon-balance/) |
| **SWAT–ABM coupled nexus model** | Process-based hydrology coupled with an NSGA-II behavioral model over ~1M farming households | [details](/models/swat-abm-nexus/) |
| **Climate Technology Cooperation Strategy Map** | Deployed decision-support platform for selecting cooperation partners | [ctis.re.kr/map](https://ctis.re.kr/map) · [details](/models/climate-tech-strategy-map/) |

Full list on the [Models & Data](/models/) page. Papers, including manuscripts under review, are on [Publications](/publications/) — every Korean-language journal article there carries an English summary.

## Contact

[deepbluelearning98@gmail.com](mailto:deepbluelearning98@gmail.com) · [bluelearning@nigt.re.kr](mailto:bluelearning@nigt.re.kr) · [Google Scholar](https://scholar.google.com/citations?hl=en&user=KSyS2SoAAAAJ) · [GitHub](https://github.com/mongbleu) · [ORCID](https://orcid.org/0009-0001-4462-0266) · [CV (PDF)](/files/CV.pdf)

I am applying to PhD programs for Fall 2027 in AI-applied environmental and hydrological modeling.

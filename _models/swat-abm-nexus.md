---
title: "SWAT–ABM Coupled Model for the Food–Water–Biodiversity Nexus"
collection: models
permalink: /models/swat-abm-nexus/
excerpt: "A process-based hydrological model coupled with an NSGA-II behavioral agent model, simulating roughly one million farming households in the Yeongsan River Basin under climate and management scenarios."
date: 2026-01-05
---

**Status:** manuscript in preparation · presented at EGU 2025 and EGU 2023 (both oral) · code release planned

## What it does

Hydrological models usually treat human water use as a boundary condition. It is not — it is a decision, made repeatedly, under uncertainty. This model couples **SWAT**, a process-based hydrological model, with a **behavioral agent-based model** whose agents solve a multi-objective problem (NSGA-II) over crop choice and water use, and simulates roughly **one million farming households** in the Yeongsan River Basin.

The coupling makes food–water–biodiversity trade-offs visible as an emergent basin outcome rather than an assumed scenario: what farmers do changes the hydrology, which changes what farmers do next.

## Inputs and outputs

| | |
|---|---|
| **Inputs** | Climate scenarios; land use and soil; agricultural census and cropping data; irrigation infrastructure; water management rules |
| **Outputs** | Basin-scale streamflow and water availability; crop production; biodiversity-relevant indicators; household-level decision trajectories |
| **Method** | SWAT ↔ ABM two-way coupling; NSGA-II multi-objective agent behavior |

## Where this is going

The NSGA-II agents optimize a fixed objective — they do not learn. The direction I am developing for doctoral research replaces the optimization core with **reinforcement learning**, coupled to a hydrology–agriculture simulator in the spirit of the [GEB framework](https://github.com/GEB-model), so that agents adapt their strategy as the basin changes and can be interrogated for what policy actually shifted behavior.

## Related output

- Jeong, Y., Jo, H. W., & Lee, W. K. *Watershed-based FWB (Food–Water–Biodiversity) Nexus Assessment using SWAT-ABM: A Case Study in the Yeongsan River Basin of the Republic of Korea.* Manuscript in preparation.
- Jeong, Y. (2025, May). Oral presentation, European Geosciences Union, Vienna.
- Jeong, Y. (2023, April). *Assessing the Sustainability in Water Use under Different Agricultural Management Planning in Yeongsan-River Basin.* Oral presentation, European Geosciences Union, Vienna.

## Funding and context

Developed within **fairSTREAM**, National Research Foundation of Korea · IIASA Strategic Initiatives (Sep 2021 – Sep 2024).

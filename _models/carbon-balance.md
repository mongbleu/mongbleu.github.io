---
title: "Local-Scale Carbon Balance Model and Typology Maps"
collection: models
permalink: /models/carbon-balance/
excerpt: "An AI-driven spatial model predicting greenhouse gas emissions at 1-hectare resolution, and a carbon balance typology that classifies every Korean local government by the structure of its sources and sinks. Open source."
date: 2026-01-10
---

**Status:** code released · two journal articles published · one under review

## What it does

Carbon neutrality is legislated nationally but implemented by local governments, which need evidence at the scale they actually govern. This model predicts greenhouse gas emissions at **1-hectare resolution** and derives a **carbon balance typology** — a classification of local governments by the structure of their emissions and sinks, so a municipality can see which mitigation lever is available to it rather than being handed a national average.

It is the model behind my M.S. thesis question: *are there carbon-neutral local regions in the Republic of Korea?*

## Inputs and outputs

| | |
|---|---|
| **Inputs** | National and local energy statistics; land cover; building and road data; forest inventory; population and industry data |
| **Outputs** | 1-ha gridded GHG emission surfaces; forest carbon sink maps; carbon balance typology by administrative unit |
| **Method** | Spatial downscaling with tree-based ML and residual modeling; sink estimation from forest inventory and land cover |

## Access

- **Source code and model** — [github.com/mongbleu/carbonBalance](https://github.com/mongbleu/carbonBalance)

## Related output

- Jeong, Y., Song, C. H., Jo, H. W., Ko, Y. J., & Lee, W. K. (2024). *Development and applicability assessment of local-scale carbon emission models to support carbon neutrality plans of local governments.* J. Climate Change Research, 15(5-1), 691–721. [DOI](https://doi.org/10.15531/KSCCR.2024.15.5.691)
- Ko, Y. J., Song, C. H., Jeong, Y., Hong, M., Kim, J., & Lee, W. K. (2024). *Development of village-level forest carbon sink map for spatial carbon sink management of the local government.* J. Climate Change Research, 15(6), 989–1000. [DOI](https://doi.org/10.15531/KSCCR.2024.15.6.989)
- Jeong, Y., Jo, H. W., & Lee, W. K. *A Regional Carbon Balance and Typology Map to Support Local Carbon Neutrality Planning in the Republic of Korea.* Under review, J. Korean Society of Forest Science.
- M.S. thesis, Korea University (2024) — [full text](https://dcollection.korea.ac.kr/public_resource/pdf/000000289241_20250511132805.pdf)
- Presented at EGU 2024 (oral), AGU 2023 (oral), KSCCR 2022 (poster).

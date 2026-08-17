---
title: "Hybrid Crown Base Height Model"
collection: models
permalink: /models/crown-base-height/
excerpt: "Allometric forest structure embedded in a machine learning model to predict and map crown base height across 36 tree species — the input layer of a crown fire simulation module. Trained model, maps, and training data released on Zenodo."
date: 2026-01-15
---

**Status:** trained model and data released · manuscript under review (*Ecological Informatics*) · Korean patent pending (KR 10-2025-0189148)

## What it does

Crown base height (CBH) — the distance from the ground to the lowest live crown — determines whether a surface fire becomes a crown fire. It is also almost never measured at scale. This model predicts and maps CBH across **36 tree species** in the Republic of Korea by embedding allometric forest structure relationships into a machine learning model, so predictions stay physically ordered in species where only a handful of plot observations exist.

The CBH surface is the input layer of a crown fire simulation module, in which a Rothermel-type fire-spread model is reformulated as a **differentiable CNN layer** — gradients flow through the physics, so the process structure constrains learning under sparse burned-area observations.

## Inputs and outputs

| | |
|---|---|
| **Inputs** | Forest inventory plot data (species, DBH, height, stand density); terrain from DEM; Sentinel-2 derived Normalized Burn Ratio (NBR); observed GIS fireline data |
| **Outputs** | Nationwide gridded crown base height maps; trained model weights; training dataset |
| **Method** | Hybrid allometric–ML model; physics-based fire spread converted to a differentiable CNN layer |

## Access

- **Trained model, maps, and training data** — Zenodo, [DOI: 10.5281/zenodo.21736584](https://doi.org/10.5281/zenodo.21736584)
- **Patent** — KR 10-2025-0189148, "System and Method for Predicting Wildfire Spread Using Artificial Intelligence and Process-Based Simulation" (filed Dec 2025, pending)

## Related output

- Jeong, Y., Jo, H. W., Roh, M., Kim, S., & Lee, W. K. *A Hybrid Allometric–Machine Learning Model for Crown Base Height Prediction in the Republic of Korea.* Under review, *Ecological Informatics* (ECOINF-D-25-04526R1).
- Jeong, Y. (2025, August). Poster, Korean Society of Forest Science — **Best Poster Award**.

## Funding and context

Developed for the Korea Forestry Promotion Institute crown fire prediction project (Apr 2024 – Dec 2025).

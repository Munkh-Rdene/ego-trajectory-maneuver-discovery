# Ego Trajectory Maneuver Discovery

This repository contains exploratory research on **unsupervised and interpretable maneuver discovery**
from normalized ego vehicle trajectories using the **Waymo Open Motion Dataset**.

## Motivation
Large-scale autonomous driving datasets contain rich trajectory information but lack explicit labels
for high-level driving maneuvers. Manual annotation is costly and subjective, motivating unsupervised,
data-driven approaches to discover recurring motion patterns directly from trajectory geometry and
kinematics.

This project explores whether simple normalization and low-dimensional trajectory representations
are sufficient to reveal interpretable ego vehicle maneuver structures.

## Core Idea
Ego vehicle trajectories are:
- recentered at their starting point
- rotated so the initial heading aligns with the x-axis
- represented using basic geometric and kinematic features

This removes global position and orientation effects, allowing maneuver structure to emerge
from trajectory shape alone.

## Research Questions
- Do normalized ego trajectories naturally organize into a small number of maneuver families?
- How stable and interpretable are these patterns under different representations?
- What level of abstraction is achievable without supervision or predefined labels?

## Dataset
- **Waymo Open Motion Dataset**
- 20-second ego vehicle trajectories extracted from diverse urban driving scenarios

## Project Status
This is an **exploratory, pre-project phase** focused on:
- data understanding
- visualization
- representation choices
- qualitative and unsupervised analysis

Clustering methods and evaluation strategies will be investigated incrementally.

## Repository Structure (planned)
```text
notebooks/     # exploratory analysis and visualization
src/           # preprocessing and feature extraction
literature/    # paper notes and summaries
figures/       # plots for analysis and writing
plan.md        # project roadmap


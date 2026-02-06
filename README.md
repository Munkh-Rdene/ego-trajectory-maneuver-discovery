# Ego-Trajectory Maneuver Discovery

This project explores interpretable discovery of ego-vehicle driving maneuvers
from real-world trajectory data using the Waymo Open Motion Dataset.

## Motivation
Many trajectory analysis tasks lack reliable labels and depend on unsupervised
methods. Rather than clustering raw trajectories directly, this project focuses
on defining **ego-vehicle maneuvers** (e.g. right turns) in a way that is invariant
to intersection geometry and orientation.

## Current Progress
- Loaded ego-vehicle trajectories from Waymo TFRecord scenarios
- Normalized trajectories by recentering and rotating by initial heading
- Defined **right-turn maneuvers geometrically** (no map labels)
- Visualized multiple normalized right turns together
- Quantified maneuver variability using final heading angle
- Distinguished maneuver geometry from execution dynamics (speed)
- Applied light unsupervised clustering to identify right-turn families

## Method Overview
1. Extract ego trajectory from each scenario
2. Normalize trajectory (translation + rotation)
3. Filter right turns based on lateral displacement
4. Analyze geometric variability (heading angle)
5. Compare speed profiles across similar geometries
6. Cluster normalized trajectories for pattern discovery

## Dataset
Waymo Open Motion Dataset (20-second scenarios).  
Raw data is **not included** in this repository.

## Status
Exploratory / research-in-progress.


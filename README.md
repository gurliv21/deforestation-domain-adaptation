# Deforestation Domain Adaptation

## Overview

This project investigates whether domain-adversarial training can improve the geographic generalization of satellite-image-based deforestation segmentation models.

A model trained on satellite imagery from one geographic region may perform poorly when evaluated on another region because of differences in vegetation, terrain, atmospheric conditions, illumination, and other domain-specific characteristics.

The goal of this project is to determine whether domain-adversarial learning can encourage a segmentation model to learn features that generalize across geographic regions.

## Research Question

> Can domain-adversarial training improve deforestation segmentation performance on geographic regions that were not seen during training?

## Approach

We will compare:

1. A standard semantic segmentation model.
2. The same segmentation model trained with domain-adversarial learning.

The models will be evaluated using geographic domain splits rather than random image splits.

## Planned Experiments

* Establish a standard segmentation baseline.
* Measure cross-region generalization.
* Implement domain-adversarial training.
* Compare baseline and domain-adapted models.
* Evaluate performance across different geographic regions.
* Analyze failure cases.
* Perform ablation experiments on domain-adversarial training.

## Evaluation

Primary metrics will include:

* Intersection over Union (IoU)
* Dice/F1 score
* Precision
* Recall

The main comparison will focus on performance on geographically held-out regions.

## Project Status

Currently setting up the dataset and experimental pipeline.

---
title: Machine-learning calibration of forward calorimeter clusters
status: Ongoing
period: 2025–present
order: 1
featured: true
summary: Neural-network energy calibration and pile-up rejection for ATLAS clusters, especially beyond tracking coverage.
tags: [ATLAS, calorimetry, machine learning, pile-up]
hero: /assets/images/calorimeter-ml.svg
hero_alt: Diagram showing calorimeter cells grouped into clusters, passed through a neural network, and used for calibrated energy, pile-up classification, jets, recoil, and missing transverse momentum.
hero_caption: Simplified analysis workflow. The production study uses the full ATLAS reconstruction and validation chain.
---

## Forward calorimeter calibration

At small angles to the beam, limited tracking coverage makes reconstruction depend heavily on calorimeter signals. Their response varies with shower development, inactive material, detector geometry, noise, and overlapping proton–proton interactions (pile-up). Better cluster calibration can improve measurements such as vector-boson scattering and those using missing transverse momentum.

## Method

With Oldřich Kepka and the ClusterML effort, I study supervised models that predict calibrated cluster energy from detector information. The most promising approach so far is a dense neural network with a heteroscedastic objective and Gaussian-mixture description, representing both the energy prediction and its varying uncertainty.

A parallel classifier estimates the pile-up contribution to each cluster. Its output can reweight clusters before constructing higher-level objects.

## Evaluation

We test energy-response linearity across energy and detector position; resolution and response tails; pile-up stability; particle and shower categories; and the resulting jet and recoil performance.

I presented the calibration and pile-up-classification studies at [BOOST 2026](https://indico.cern.ch/event/1574970/contributions/7103178/).

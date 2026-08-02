---
title: Machine-learning calibration of forward calorimeter clusters
status: Ongoing
period: 2025–present
order: 1
featured: true
summary: Developing neural-network methods to improve the energy calibration and pile-up rejection of ATLAS calorimeter clusters, especially where tracking information is unavailable.
tags: [ATLAS, calorimetry, machine learning, pile-up]
hero: /assets/images/calorimeter-ml.svg
hero_alt: Diagram showing calorimeter cells grouped into clusters, passed through a neural network, and used for calibrated energy, pile-up classification, jets, recoil, and missing transverse momentum.
hero_caption: Simplified analysis workflow. The production study uses the full ATLAS reconstruction and validation chain.
---

## Why the forward calorimeter matters

Many ATLAS measurements rely on particles produced at small angles to the beam. In this forward region, the inner detector does not provide the same tracking coverage available in the central detector, so calorimeter signals carry much of the reconstruction task. A small improvement at the cluster level can therefore influence a wide range of measurements, including vector-boson scattering and analyses involving missing transverse momentum.

The difficulty is that a cluster's measured response depends on more than the energy of the particle that produced it. Shower development, inactive material, detector geometry, noise, and overlapping proton–proton interactions all shape the signal.

## What I am studying

With Oldřich Kepka and the ClusterML effort, I investigate supervised models that learn a calibrated cluster energy from detector-level information. The most promising approach so far uses a dense neural network with a heteroscedastic objective and a Gaussian-mixture description. This lets the model represent both a central prediction and the non-uniform uncertainty of a highly stochastic calorimeter response.

A parallel classification task estimates how much of a cluster is associated with pile-up rather than the hard-scatter collision. The output can be used to reweight cluster contributions before higher-level objects are constructed.

## How success is evaluated

A useful calibration must do more than improve an average response. We examine:

- energy-response linearity across energy and detector position;
- resolution and the tails of the response distribution;
- stability as the amount of pile-up changes;
- performance for different particle and shower categories; and
- downstream behavior when the calibrated clusters are used to build jets and recoil.

This work was presented at [BOOST 2026](https://indico.cern.ch/event/1574970/contributions/7103178/), with the latest status of the calibration and pile-up-classification studies.

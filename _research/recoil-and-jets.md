---
title: From calibrated clusters to jets and hadronic recoil
status: Ongoing
period: 2025–present
order: 2
featured: true
summary: Testing whether improvements learned at the calorimeter-cluster level remain useful once signals are assembled into jets, recoil, and missing transverse momentum.
tags: [ATLAS, jets, hadronic recoil, missing momentum]
---

Improving an individual calorimeter cluster is only valuable if that improvement survives the rest of the reconstruction chain. This project follows the machine-learning-calibrated clusters into the physics objects that analyses actually use.

## The hadronic recoil

The hadronic recoil is the vector sum of reconstructed activity balancing a well-measured reference object, such as a photon or a vector boson. It is an especially sensitive diagnostic: biases, extra pile-up energy, and resolution effects from many detector signals accumulate in one observable.

Accurate recoil reconstruction matters for precision measurements and for searches with missing transverse momentum. The study therefore asks whether learned calibration and pile-up weights yield a response that is more linear, narrower, and more stable across event conditions.

## From local to global performance

I evaluate the new cluster definitions in jet reconstruction and event-level balance. The comparisons are made against established calibrations using common samples and selections, so a gain cannot be attributed merely to a change in the event population.

The central questions are:

- Do reconstructed jets recover the reference energy more accurately?
- Does the response remain stable with increasing pile-up?
- Are improvements uniform across jet momentum and detector pseudorapidity?
- What happens to soft activity and the missing-transverse-momentum resolution?

This downstream validation is deliberately separate from model training. It tests whether the network learned a detector correction that generalizes, rather than only optimizing its cluster-level target.

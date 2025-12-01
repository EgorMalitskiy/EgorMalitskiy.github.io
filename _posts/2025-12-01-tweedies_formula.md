---
layout: default # Refers to the _layouts/default.html file you created
title: "Tweedies formula"
date: 2025-12-01 10:00:00 -0500
categories: mathematics
---

## Tweedies formula
In generative modeling we are given samples $x_0$ from a unknown distribution (e.g. images). The standard DDPM formulation is: We add noise until the samples are indistinguashable from a pure Gaussian sample, and then try to reverse this process. Essentially, we apply a "noising" transformation for each sample $x_0$ given by: 
$$x_1 = x_0 + \epsilon, \quad \text{ where } \epsilon \sim \mathcal{N}(x_0, \sigma ^2 I_d)$$


### Bayesian Perspective




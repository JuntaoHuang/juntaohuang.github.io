---
layout: page
permalink: /code/
title: Code
description:
nav: true
nav_order: 4
---


<style>
.post-title
{
  display: none;
}
</style>

##### **Open-source Packages**

---

###### **1. [AdaM-DG](https://github.com/JuntaoHuang/adaptive-multiresolution-DG)**

---

This C++ package implements adaptive sparse grid and multiresolution DG methods for high-dimensional PDEs. It is designed to handle nonlinear equations efficiently in arbitrary dimensions, while keeping the computational cost manageable through hierarchical basis representations and adaptive refinement. For more details on the algorithm and implementation, please refer to our review paper:

- [Adaptive sparse grid discontinuous Galerkin method: review and software implementation](https://link.springer.com/article/10.1007/s42967-023-00268-8)

---

###### **2. [multiscale-chemical-reaction](https://github.com/JuntaoHuang/multiscale-chemical-reaction)**
  
This Python package provides data-driven tools to identify model parameters and mechanisms for multiscale chemical reaction systems. The implementation supports learning physically meaningful reaction models from data and is aligned with thermodynamic and structural constraints in the governing equations. For more details on the algorithm, please refer to our paper:
- [Data-driven discovery of multiscale chemical reactions governed by the law of mass action](https://www.sciencedirect.com/science/article/abs/pii/S0021999121006380)

---

###### **3. [entangled-network](https://github.com/JuntaoHuang/entangled-network)**

This repository contains C++ codes for modeling the mechanics (strength and toughness) of entangled networks. For more details on the modeling, algorithm and implementation, please refer to our paper:

- [Topological Mechanics of Entangled Networks](https://arxiv.org/abs/2509.17813)

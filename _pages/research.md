---
layout: page
permalink: /research/
title: Research
description:
nav: true
nav_order: 2
---


<style>
.post-title
{
  display: none;
}

/* Offset in-page anchors for sticky header */
a[id^="topic-"] {
  display: block;
  position: relative;
  top: -65px;
  visibility: hidden;
}
</style>

##### **Research**

My research interest lies in **scientific computing**, **numerical analysis**, **multiscale modeling**, and **data science**. Specific topics of interest include:
- [**Machine learning for multiscale modeling**](#topic-ml-multiscale)
- [**Network modeling for polymers and architected materials**](#topic-network-modeling)
- [**Sparse grid methods for high-dimensional PDEs**](#topic-sparse-grid)
- [**High-order numerical schemes for hyperbolic equations**](#topic-hyperbolic)
- [**Lattice Boltzmann methods for fluid simulations**](#topic-lbm)


---

<a id="topic-ml-multiscale"></a>
##### **1. Machine learning for multiscale modeling**

Modeling multiscale systems remains a fundamental challenge in computational mathematics and scientific applications. These systems often exhibit complex and high-dimensional dynamics across multiple scales, making it difficult to achieve accurate predictions without prohibitive computational costs. Traditional coarse-grained approaches, which typically rely on empirical closure models, often fall short of capturing the detailed fine-scale physics essential for predictive accuracy.

Recent advancements in machine learning (ML) have opened promising avenues for computational science, yet ML models are often criticized as black boxes with limited interpretability and robustness. This lack of transparency limits their utility in modeling and simulation. For ML models to become a reliable tool in multiscale modeling, a central challenge emerges: **How can we embed physical constraints and mathematical structures into ML models to ensure
well-posedness?** My research tackles this challenge by developing accurate ML models for multiscale systems,
with applications in kinetic theory, hydrodynamic modeling, and polymer networks in materials
science. The overarching goal is to go beyond phenomenological insights and enable accurate
modeling of multiscale systems.

###### **1.1 Machine learning moment closures for kinetic transport**

Kinetic equations provide mesoscale descriptions of non-equilibrium transport, but direct simulation is expensive in high-dimensional phase space. I develop **structure-preserving ML moment closures** with provable properties such as **hyperbolicity**, Galilean invariance, and physically meaningful characteristic speeds.

Related works:
- *Learning thermodynamically stable and Galilean invariant partial differential equations* (J. Non-Equilib. Thermodyn., 2021)
- *Data-driven discovery of multiscale chemical reactions governed by the law of mass action* (J. Comput. Phys., 2022)
- *Machine learning moment closure models for the radiative transfer equation I: directly learning a gradient based closure* (J. Comput. Phys., 2022)
- *Machine learning moment closure models for the radiative transfer equation II: enforcing global hyperbolicity in gradient based closures* (SIAM Multiscale Model. Simul., 2023)
- *Machine learning moment closure models for the radiative transfer equation III: enforcing hyperbolicity and physical characteristic speeds* (J. Sci. Comput., 2023)
- *Hyperbolic machine learning moment closures for the BGK equations* (SIAM Multiscale Model. Simul., 2025)
- *Machine learning-based moment closure model for the linear Boltzmann equation with uncertainties* (Comput. Methods Appl. Mech. Engrg., 2026)



###### **1.2 Shallow water moment models**

Classical shallow water equations are efficient but lose important vertical structure. The shallow water moment equations is a new class of models derived using vertical moments information, I study model classes with provable **rotational invariance** and **hyperbolicity**.

Related works:
- *On the rotational invariance and hyperbolicity of shallow water moment equations in two dimensions* (SIAM J. Math. Anal., 2025)
- *Moment-enhanced shallow water equations for non-slip boundary conditions* (arXiv, 2025)

<a id="topic-network-modeling"></a>
##### **2. Network modeling for polymers and architected materials**

Entangled networks are ubiquitous in tissues, polymers, and fabrics. However, their mechanics remain insufficiently understood due to the complexity of the topological constraints at the network level. Here, I develop **mesoscale discrete network models**, a mathematical framework that models entangled networks as graphs, capturing topological constraints of entanglements. This framework establishes fundamental principles of linking topology to mechanics of entangled networks and offers a foundational tool for designing reconfigurable materials.

Related works:
- *Topological mechanics of entangled networks* (arXiv, 2025)

---

<a id="topic-sparse-grid"></a>
##### **3. Sparse grid methods for high-dimensional PDEs**

The discretization of PDEs by conventional numerical schemes is typically limited to problems with up to three dimensions. The reason is the so-called **curse of dimensionality**, which refers to the fact that the computational
cost and storage scale as $O(N^d)$ for a $d$-dimensional problem with $N$ grid points in each dimension. 
To mitigate the curse of dimensionality, I develop adaptive sparse grid discontinuous Galerkin (DG) methods. This includes efficient treatment of nonlinear terms using interpolatory multiwavelets and multiresolution analysis, as well as open-source software implementation.

Related works:
- *An adaptive multiresolution discontinuous Galerkin method with artificial viscosity for scalar hyperbolic conservation laws* (SIAM J. Sci. Comput., 2020)
- *An adaptive multiresolution interior penalty discontinuous Galerkin method for wave equations in second order form* (J. Sci. Comput., 2020)
- *An adaptive multiresolution ultra-weak discontinuous Galerkin method for Schrodinger equations* (Commun. Appl. Math. Comput., 2020)
- *An adaptive sparse grid local discontinuous Galerkin method for Hamilton-Jacobi equations in high dimensions* (J. Comput. Phys., 2021)
- *A class of adaptive multiresolution ultra-weak discontinuous Galerkin methods for some nonlinear dispersive wave equations* (SIAM J. Sci. Comput., 2022)
- *Adaptive sparse grid discontinuous Galerkin method: review and software implementation* (Commun. Appl. Math. Comput., 2024)
- Software: [AdaM-DG](https://github.com/JuntaoHuang/adaptive-multiresolution-DG)

---

<a id="topic-hyperbolic"></a>
##### **4. High-order numerical schemes for hyperbolic equations**

Hyperbolic equations are an important class of PDEs, which describes physical phenomena where information or signals travel with finite speeds. They are typically used to describe wave propagation or conservation laws in various scientific and engineering fields, including chemically reactive flows, radiation hydrodynamics, inviscid gas dynamics with relaxation, nonlinear optics, and so on. I develop robust high-order methods for hyperbolic equations, including structure-preserving time discretizations and high-order boundary treatments on Cartesian grids.

##### **4.1 Structure-preserving time discretizations**

I design and analyze high-order **bound-preserving** and **asymptotic-preserving** time integrators, including IMEX and exponential-type schemes for stiff source terms and multiscale regimes.

Related works:
- *A second-order asymptotic-preserving and positivity-preserving DG scheme for the Kerr-Debye model* (Math. Models Methods Appl. Sci., 2017)
- *Bound-preserving modified exponential Runge-Kutta DG methods for scalar hyperbolic equations with stiff source terms* (J. Comput. Phys., 2018)
- *Positivity-preserving time discretizations for production-destruction equations with applications to non-equilibrium flows* (J. Sci. Comput., 2019)
- *A third-order unconditionally positivity-preserving scheme for production-destruction equations* (J. Sci. Comput., 2019)
- *On the stability of strong-stability-preserving modified Patankar Runge-Kutta schemes* (ESAIM: Math. Model. Numer. Anal., 2023)
- *Bound-preserving discontinuous Galerkin methods with modified Patankar time integrations for chemical reacting flows* (Commun. Appl. Math. Comput., 2023)
- *Coupling conditions for linear hyperbolic relaxation systems in two-scales problems* (Math. Comp., 2023)
- *Uniform accuracy of IMEX-RK methods for linear hyperbolic relaxation systems* (J. Sci. Comput., 2025)
- *Uniform accuracy of IMEX-BDF methods for linear hyperbolic relaxation systems* (Math. Comp., 2025)



##### **4.2 High-order numerical boundary conditions for finite difference methods on Cartesian grids**

In finite difference methods, Cartesian grids are widely used since the grid generation is simple and the numerical schemes are usually more efficient and simple than those on body-fitted grids. However, the challenge with Cartesian grids is to accurately impose the boundary conditions while retaining the stability under the standard CFL conditions determined by the interior schemes. For high-order methods on Cartesian grids with irregular boundaries, I extend inverse Lax-Wendroff boundary treatments to high-order RK of arbitrary order and IMEX-RK schemes without requiring intermediate-stage boundary data.

Related works:
- *Boundary treatment of high order Runge-Kutta methods for hyperbolic conservation laws* (J. Comput. Phys., 2020)
- *Boundary treatment of implicit-explicit Runge-Kutta method for hyperbolic systems with source terms* (J. Comput. Phys., 2020)

---

<a id="topic-lbm"></a>
##### **5. Lattice Boltzmann methods (LBM) for fluid simulations**

The LBM is a class of kinetic numerical methods for fluid simulations. Instead of solving the Navier-Stokes equations directly, this numerical method is motivated by the discrete velocity Boltzmann equation and evolves with probability distribution functions. The macroscopic quantities are then obtained by taking moments of distribution functions. The challenge of transitioning from kinetic to fluid models is particularly intriguing. I work on **boundary and interface treatments** of the LBM, using **asymptotic analysis** to connect kinetic and macroscopic models for complex boundary conditions on curved boundaries.

Related works:
- *Boundary conditions of the lattice Boltzmann method for convection-diffusion equations* (J. Comput. Phys., 2015)
- *On initial conditions for the lattice Boltzmann method* (Commun. Comput. Phys., 2015)
- *Second-order curved boundary treatments of the lattice Boltzmann method for convection-diffusion equations* (J. Comput. Phys., 2016)
- *Lattice Boltzmann method for convection-diffusion equations with general interfacial conditions* (Phys. Rev. E, 2016)
- *Second-order curved interface treatments of the lattice Boltzmann method for convection-diffusion equations with conjugate interfacial conditions* (Comput. Fluids, 2017)
- *Boundary conditions for kinetic theory based models I: Lattice Boltzmann models* (SIAM Multiscale Model. Simul., 2019)
- *Lattice Boltzmann method for stochastic convection diffusion equations* (SIAM/ASA J. Uncertain. Quantif., 2021)


---

For complete publication details, please see the [Publications](/publications/) page.

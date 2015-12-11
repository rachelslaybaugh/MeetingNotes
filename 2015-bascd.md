[Bay Area Scientific Computing Day](https://sites.google.com/a/lbl.gov/bascd-2015/home)

LBNL

11 December, 2015

### <a name="top">Speakers
1.  [Juliane Mueller, LBL](#mueller)
2.  [Diep Nguyen, UCB](#nguyen)
3.  [Daniele Schiavazzi, Standord](#schiavazzi)
4.  [Jakub Cerveny, LLNL](#cerveny)
5.  [Noemi Petra, UC Merced](#petra)
6.  [Ariful Azad, LBL](#azad)
7.  [Ke Wei, UC Davis](#wei)
8.  [Moe Kahlil, SNL](#khalil)
9.  [Victor Minden, Standford](#minden)
10. [Andrea Dotti, SLAC](#dotti)

Kathy's opening remarks touched on computing things happening at the lab: national strategic computing initiative and exascale computing. Here NERSC is getting machines up and running. Develop lots of great algorithms for the new machines. 


#### <a name="mueller"> Surrogate Model Algorithms for Computationally Expensive Multi-objective Optimization problems, Juliane Mueller

- vector of objectives; want to minimize; often each entry is in conflict with one another
- Pareto-optimal is the line of function value combinations that make a minimum sort of line
- goal: find Pareto front; decision vector domination is when one value is better than all others
- once you get the front, now you have to choose which solution to use
- hard b/c all of the function evaluations is hard; the f_i are black-box; usually need thousands of function evaluations. The goal is get an approximate Pareto front in a few hundred evals
- Surrogate models! cheap approx of real objective function
- currently she is using deterministic models; no noise
- using radial basis function surrogate model: s(x) = \sum_j \lambda_j \phi (||x - x_j||_2) + p(x)
- here \phi -is cubic radial basis function, p(x) is the polynomial tail, x_j is already evaluated points, get parameters from solving a linear system
- has algorithm steps
- balance between local and global search
- get the evaluations and input values, how do you determine which input values to use next?
- after you have some points on the Pareto front, you decide you want some fill in points, you choose the objective values and guess input values to try to fill in the gap
- you also perturb the non-dominated points to find others nearby
- it is helpful for real engineering problems to know the Pareto front so engineer can make informed decision about what is important
- gave numerical example result, local global balance
- they key is that the surrogate models are cheap compared to the real ones
- they'd like to look at problems with many more objectives and larger dimensions; want to compare to state-of-the-art MO algos

[Speaker List](#top)



#### <a name="nguyen"> Reproducibility at Extreme Scale, Diep Nguyen

- sources of non-reproducibility: going very fast
- motivation: several
- solution: fix order of computation (can be expensive), try to eliminate and reduce rounding errors
- objectives: bit-wise identical results, independent of ordering in parallelization, no sever loss of accuracy
- something about discarding bits with memory boundaries
- [reproblas](http://bebop.cs.berkeley.edu/reproblas/index.php): on bebop website
- reproblas has rigorous reproducibility, but is 8x slower, worse for higher order ops. looking to see if they can save with places where they don't need high accuracy and they don't need to worry about totally random evaluation order
- can be applied to gemv and gemm, not sure about LU or QR factorization; investigating

[Speaker List](#top)



#### <a name="schiavazzi"> Assimilation and Propagation of Clinical Data Uncertainty in Cardiovascular Modeling, Daniele Schiavazzi

- multiscale modeling of single-ventricle pathologies, UQ-based approach
- this is a big problem for babies
- multi-scale modeling; CFD models; use advanced FE for CFD, implicit coupling with circulation network, stabilization at coupled surfaces to prevent backflow divergence. 
- study 1: propagation of uncertainty in outflow 
- iterative simulation is too expensive; train a surrogate model (MCMC), use a model inversion based on empirical hydraulics
- use MCMC to estimate PDFs of inputs that determine things, surrogate is Gaussian Process model, check the distributions
- model pre- and post-op scenarios and use for global clinical indicators
- this work could have lessons that translate into our flow problems
- [simvascular](simvascular.github.io) is a completely open source tool set to do all of this

[Speaker List](#top)



#### <a name="cerveny"> Nonconforming Mesh Refinement for High-Order Finite Elements, Jakub Cerveny

- high-order shock hydrodynamics, applied to NIF
- BLAST (physics) -> MFEM (finite elements) -> HYPRE (linear algebra)
- goal is to enable nonconforming amr in BLAST; [MFEM](http://mfem.org) is free, lightweight, scalable
- nonconforming refinement allows hanging nodes
- FE space cut along coarse-fine interfaces; define constrained FE space with some DOFs eliminated
- y = Px, y is nonconforming space of DOFs (conforming + slaves) and x is conforming space; P = [I W], W is interpolation for slave DOFs
- need to support curved meshed, parallelization, anisotropic refinement
- how do you make P? use interpolation of nodal FEMs using a local interpolation matrix, Q
 -issue: some slave DOFs might depend on other slaves (slaves are the hanging nodes that cause the problems)
- start by making P for constrained rows, then for linearly-constrained, the next layers down
- structs for elements, vertices, and faces linked with pointers is hard to maintain in 3D
- they drop most of the pointers and keep most of the hierarchy in associative maps; they use a hashing system to keep track of intermediate nodes and edges - looks more efficient; one data structure does not have to keep all of the information straight in the same way; looks like there is more of just needing to know about your neighbors
- however, sometimes you get invalid mesh; sometimes need to add more refinement to make the mesh valid for use with FEM to get continuous solutions
- what about parallelization? there's some standard Z curve thing, they change that a little bit to get something that is a Huber curve (looks U-ish) that is apparently better.
- need ghost elements to create P in parallel
- Also have load balancing by repartioning the space-filling curve
- good both strong and weak scaling - cool plot of how they did that!
- applying to Lagrangian shock hydrodynamics in BLAST, part way through their implementation
- also looking at other applications like electrodynamics, high-order DG advection, H(div) radiation diffusion

[Speaker List](#top)



#### <a name="petra"> Large-Scale Bayesian Inverse Problems Governed by Differential and Differential-Algebraic Equations, Noemi Petra

- inverse problems: ill-posed, under-determined
- given observations d, find m such that d \approx f(m)
- Bayesian approach is f(m)(+e) = d; m and d are random variables; solution is a PDF that is a function of m.
- want to figure this out when f() is expensive
- she is going a bit too fast for me to follow; lots of info and slides and I am not familiar with this stuff
- assume additive Gaussian noise, something about the properties of the covariance operator
- get a deterministic inverse problem with appropriately weighted norms
- MAP (maximum a posteriori) point requires...
- Metropolis-Hastings Algorithm to sample the posterior
- I tuned out b/c I really didn't have enough background to follow and just got lost
- applied to Nonlinear Stokes ice sheet model

[Speaker List](#top)



#### <a name="azad"> Parallel sparse matrix-matrix multiplication and its use in triangle counting and enuermation, Ariful Azad




[Speaker List](#top)



#### <a name="wei"> Guarantees of Riemannian Optimization for Low Rank Matrix Recovery, Ke Wei




[Speaker List](#top)



#### <a name="kahlil"> Probabilistic Interference of Model Parameters and Missing High-Dimensional Data Based on Summary Statistics




[Speaker List](#top)



#### <a name="minden"> Fast Spatial Gaussian Process Maximum Likelihood Estimation via Skeletonization Factorizations, Victor Minden 




[Speaker List](#top)



#### <a name="dotti"> Modernizing large scale software for parallel hardware: the experience with GEANT 4, Andrea Dotti 




[Speaker List](#top)


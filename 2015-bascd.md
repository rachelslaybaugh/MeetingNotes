Bay Area Scientific Computing Day
[https://sites.google.com/a/lbl.gov/bascd-2015/home](https://sites.google.com/a/lbl.gov/bascd-2015/home)

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

Kathy's opening remarks touched on computing things happening at the lab: national strategic computing initative and exascale computing. Here NERSC is getting machines up and running. Develop lots of great algorithms for the new machines. 


#### <a name="mueller"> Surrogate Model Algorithms for Computatinally Expensive Multi-objective Optimization problems, Juliane Mueller

- vector of objectives; want to minimize; often each entry is in conflict with one another
- Pareto-optimal is the line of function value combinations that make a minimum sort of line
- goal: find Pareto front; decision vector domination is when one value is better than all others
- once you get the front, now you have to choose which solution to use
- hard b/c all of the function evaluations is hard; the f_i are black-box; usually need thousands of function evaluations. The goal is get an approximate pareto front in a few hundred evals
- Surrogate models! cheap approx of real objective function
- currently she is using deterministic models; no noise
- using radial basis function surrogate model: s(x) = \sum_j \lambda_j \phi (||x - x_j||_2) + p(x)
- here \phi -is cublic radial basis function, p(x) is the polynomial tail, x_j is already evaluated points, get parameters from solving a linear system
- has algorithm steps
- balance between local and global search
- get the evaluations and input values, how do you determine which input values to use next?
- after you have some points on the pareto front, you decide you want some fill in points, you choose the objective values and guess input values to try to fill in the gap
- you also perturb the non-dominated points to find others nearby
- it is helpful for real engineering problems to know the pareto front so engineer can make informed decision about what is important
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
- reproblas has rigorous reproducibility, but is 8x slower, worse for higher order ops. looking to see if they can save with places where they don't need high accruacy and they don't need to worry about totally random evaluation order
- can be applied to gemv and gemm, not sure about LU or QR factorization; investigating
- 


[Speaker List](#top)



#### <a name="schiavazzi"> Nonconforming Mesh Refinement for High-Order Finite Elements, Daniele Schiavazzi




[Speaker List](#top)



#### <a name="nguyen"> Reproducibility at Extreme Scale




[Speaker List](#top)



#### <a name="nguyen"> Reproducibility at Extreme Scale




[Speaker List](#top)


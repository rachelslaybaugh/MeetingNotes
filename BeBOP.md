## BeBOP meetings

### index
* [2015.08.19](#2015-08-19)

***


#### <a name="2015.08.19">2015.08.19

Nahid Emad (Maison de La Simulation / U of Versailles)
-----------
Unite and Conquer Approach for High Scale Numerical Computation; Application to Krylov Methods

- autotuning
- hybridize numerical methods to solve large scientific applications, asynchronously with each of them auto-adapted

- programming paradigms:
  - multicore to many core; high degree of hierarchy (nodes, memory)
  - component approach 
  - graph of tasks: very coarse grain components/tasks (data flow or PGAS-like data parallelism)
- what methods?
  - avoid synchronous communication
  - introduce fault tolerance
  - restarted krylov subspace methods - Arnoldi; Saad (ERAM) and Sorrensen (IRAM); both have problems with clustered eigenvalues
  - unite and conquer approach: combine several iterative methods to accelerate the convergence of them, e.g. ERAM + GMRES + ... or Projection method + convergence accelerator + ...
  - Saad (chebychev acceleration), Brezinski (hybrid)
  - GMRES/LS-Arnoldi for linear. Multileve parallelism; asynch comm; fautl tol; load balance
- (missed most of this b/c of buying a bus ticket)
- look up MIRAM method; could be very useful
- used PETSc/XMP?/YML
- also did MERAM
- concerns about reproducibility of results (ordering of things), debugging, and repeatability of performance

<next person>
- Auto-tuned Krylov methods, some correlated goals
- auto-tuning the subspace size
- incomplete orthogonalization; # of vectors orthogonalized at run time can be auto-tuned
- past: auto-tune of increase/decrase subspace size; restart trigger
  - increasing subspace size has a memory impact we need to think about
  - auto-tuning increase depending on levels of memory
- results of auto-tuning incomplete orthogonalization is very promising
  - auto-tuning the orthog is better than restart alone or orthog+restart in some cases - seems to vary, esp with larger core counts
  - incomplete arnoldi outperforms arnoldi; arnoldi benefits from hybergraph optimization
  - challenges with fitting matrices on gpus for testing and realy having impact for some of these methods
- ERAM restart strategies
  - (Calvin Christophe)
  - asynchronous iterative restart methods
  - hybrid method better than gmres(m) itself
- new programming paradigms are needed to really sort out some of these ideas and take advantage of things




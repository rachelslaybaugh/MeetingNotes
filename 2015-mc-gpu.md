Workshop on programming techniques for accelerators applied to Monte-Carlo simulations

Ecole Polytechnique; Paris, France

10 July, 2015

### Speakers
* [1: Francois Courteillei, NVIDIA](#nvidia)
* [2: Ryan Bergmann, PSI](#psi)
* [2: F.X. Hugot, CEA Saclay](#cea1)
* [2: Emeric Brun, CEA Saclay](#cea2)

#### <a name="nvidia">Francois Courteillei (NVIDIA): Programming Models for Pre-Exascale Systems

- talking about pre-exascale systems: Jaguar, Titan Summit
- two of the new systems are from IBM and will integrate GPUs, the other will use XeonPhi
- NVLink HIgh-Speed GPU Interconnect. 
  2014 Kepler (x86, arm64, power cpu); 2016 Pascap GPU uses NVLink. 
  A unified memory system that will use the high-speed interconnect.
- Considering how much of your program is serial. Do you need a power cpu? 
  Or, is it mostly parallelized so you just need low power, you could use arm64.
- system sketch for hardware
- Directions of future architectures:
  - likely to continue the same trends as today
  - higher level of parallelism 
    (throughputs up, latencies about the same, therefore need to increase concurrency)
  - vector execution (SIMD, SIMT)
  - Vector memory access (coalesched/spatially-local)
  - Vector lengths are getting longer
  - memory hierarchy is becoming more complex
  - scalar performance is not increasing (will start decreasing)
- Software must
  - clearly identify 3 levels of concurrency: MPI/PGAS between NUMA/UMA memory regions;
    threading within the NUMA/UMA (implementation is important; OpenMP, OpenACC);
    SIMDization at the low level
  - arithmetic and memory access parallelism
  - coalesce memory access: minimize # of cache lines requested
  - coherent control flow w/in vectors
- Models: MPI + X (regular languages / approaches like C++, OpenACC, etc.); 
  MPC (mpc.paratools.com; parallel framework; more like MPI and OpenMP together; takes care of data on socket w/ threads, etc.) + X; 
  LEGION (nvidia research project; legion.stanford.edu; intelligent runtime) + DSL 
- Want not only for code to run on different architectures, but also want performance portability
- Legion is w/ Stanford and LANL
- open ecosystem: libraries; compilers; languages all for power cpu, x84, and arm
- Libraries: easiest way to get speedups out of the box for GPUs
- AmgX (preconditioners) , ArrayFire, MAGMA, cuBLAS, Thrust (C++ stl17 proxy)
- New buzzword: deep learning, neural network for learning the deep network
- Caffe dev branch: CUDNN, does neural network acceleration. Used by major tech companies.
- Existing codes must adapt to accelerated computing: 
  big shift to thousands of threads w/in a node
- (PGI was purchased by NVIDIA last year)
- OpenACC is a consortium. Directives manage data movement, parallel execution,
  and loop mappings. Works on CPU, GPU, and MIC.
- Deep copy requires transfer over PCIe, which is the slowest xfer inside the node. 
  Trying to avoid having to do that if you can...
- LULESH is OpenMP implementation; easy to switch to OpenACC
- Key diff in MP and ACC: ACC has "performance portability" while MP has "functional portability"
- Slide mapping OpenACC to OpenMP functionality.
- Languages slide looks useful (to keep track of all the names...)


#### <a name="psi">Ryan Bergmann (PSI): tutorial on WARP



#### <a name="cea1">F.X. Hugot (CEA Saclay): tutorial on WARP



#### <a name="cea2">Emeric Brun (CEA Saclay): tutorial on WARP

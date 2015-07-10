Workshop on programming techniques for accelerators applied to Monte-Carlo simulations

Ecole Polytechnique; Paris, France

10 July, 2015

### Speakers
* [1: Francois Courteillei, NVIDIA](#nvidia)
* [2: Ryan Bergmann, PSI](#psi)
* [3: F.X. Hugot, CEA Saclay](#cea1)
* [4: Emeric Brun, CEA Saclay](#cea2)
* [6: G. Grasseau, Ecole Polytechnique](#ecole-poly)

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
- OptiX does acceleration automatically
- fission bank map slide clarifies the text from the annals paper that I did not quite get...
- Q: could we run several batches concurrently and synchronize at the end? 
  A: Yes in principle, but you would need to coordinate the fission bank 
  (as long as you do it after the fission bank is converged). Could be worth thinking about...
- Knowing which thing we are bound by (in this case it is largely latency followed by
  memory I think) helps dictate good strategies.


#### <a name="cea1">F.X. Hugot (CEA Saclay): Using CUDA/Thrust for NVIDIA GPU...
- CPUs: few and heavy threads; fast flow
- GPUs: light and numerous (32) threads doing exactly the same operations (SIMT) 
  to avoid complexity, using several blocks of threads to allow filling 
  latencies, slower monoprocessors flow
- Maxwell is newest gpu, Pascal is next
- Outline of what ability is incorporated for each compute capability (cc) level
- Good chip layout explanation
- Each core only runs 1 thread; 
  the scheduler manages how a warp of 32 threads get assigned to cores
- Issues for GPUs:
  - PCIe transfer delay: use pinned memory and hide transfers to minimize
  - coalescence and data alignment
  - divergence (if, switch, etc.)
- Nvidia-smi get your GPU name and model. 
  Device Query to get your GPU specs. 
  Bandwidth Test to get your PCIe bandwidth
- nvcc: compiler; cuda-gdb: debugger; NVprof: text profiler; etc.
- Cons of objects: polymorphism extends poorly to SIMT; side effects are not always clear; 
  inheritance increases code dependencies
- (missed one)
- Cons of templates: syntax in C++ is awful
- Map of algorithms from STL to Thrust
- Pointers are required in GPUs (can not use reference until Uniform Memory is generalized)
- Pointers are hard to do properly, but CUDA MemCheck can help
- Set of 3 examples
- Can compile this same code for different architecture with different compiler commands.
  Using that put the same code on GPU, CPU, TBB (12 cores x 2), OpenMP (12 cores x 2), and MIC
- nvvp: visual profiler tells you all kinds of useful things
- The text profiler gives similar information. It is of course less pretty,
  but seems more informative.
- Punchline: cuda/thrust provides access to large speedups for gpus, cpus with tbb or openmp,
  or on mics. Allows structures programming; can get preliminary results.


#### <a name="cea2">Emeric Brun (CEA Saclay): Status of the development of Patmos



#### <a name="ecole-poly">G. Grasseau (Ecole Polytechnique): The Matrix Element Method (MEM) for the Higgs boson data analysis on GPUs

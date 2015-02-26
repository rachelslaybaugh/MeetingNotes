Worklog for adding CRAM to PyNE

### Meeting list
* [Meeting: 2015/02/09](#meeting-20150209)

***

### Background information: 2015/02/25
[mostly taken from PPHW's thesis, some info confirmed from my memory by wikipedia].
* Activation: an atom captures a neutron, becomes a new isotope, and enters an
  excited state and becomes radioactive. This excited atom will decay. 
  If it decays be something other than gamma emission, it will then become
  another isotope or element.
* Transmutation: the conversion of one element or isotope to another
* A material's radioactivity comes from the concentration of a given isotope
  mulitplied by its decay constant (\lambda = ln(2)/t_{1/2})
* The production rate of isotope i from j, P_{j\rightarrow i} can be through 
  activation or decay.
* $P_{j \rightarrow i}$ activation = \sigma^{j\rightarrow i}_g \phi_g
* P_{j \rightarrow i} decay = \lambda_j b_{j \rightarrow i} (b is branching
  ratio)
* Together, this means that dN_i/dt = \num_{j=1}^n P_{j \rightarrow i} N_j(t)
                                    - \num_{k=1}^n P_{i \rightarrow k} N_i(t)

Our code will need to:
* build the activiation tree given the starting isotopes
* solve the problem (with CRAM; that algorithm is implemented)

-----------------
Useful details about PyNE interface.
The `Material Class` is in `pyne/src/material.cpp` and `pyne/pyne/material.pxd`,
pyne/pyne/material.pyx`, and `pyne/pyne/cpp_material.pxd`:



### Meeting: 2015/02/09
On PyNE dev call
* We'll put this as its own branch for now

Entry points for the code:
* add method to `pyne/pyne/transmute` directory, which currently contains
  `chainsolve.py` and `origen22.py`
* there is also a decay method in `pyne/source/material.cpp`
* material could have a transmute function that calls the transmute class.
* we could have a decay matrix that is pre-assembled

Things we will need:
* our own data and benchmarks
* group structures in PyNE
* be able to use transmute and decay interchangably

For now, focus on decay only

Note: it is better to put in multiple small pull requests than one large one.

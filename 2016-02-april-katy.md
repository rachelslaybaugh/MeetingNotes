Feb 1 2016
-----------

Pronghorn has been extended for molten salts in pebbels. The TMSR benchmarcks in China are a useful thing. Lots of codes to compare.

Moose -> Pronghorn and Yak
- materials are assigned by mesh index

Pronghorn handles the interesting physics 
- diffusion neutronics model
- neutronics material holds xsecs and Ds, etc.
- TH Darcy flow

Yak
- Sn (kernel used by Rattlesnake)

People
- Xin: approx diffusion model in comsol; linked to peb bed ht xfer but not flow; can only do comsol
- Manuele: coupled TH and Serpent

Feb:
- tests pass (for extended Pronghorn)
- Create meshes / materials / boundary conditions / cross section data [f(t): Serpent at 50 incr temps - 8g data (bounds) from Manuele]

Mar:
- methods paper
- run tmsr benchmarks with Pronghorn

April:
- run more tmsr benchmarks with Pronghorn


May:
- run more tmsr benchmarks with Pronghorn


June:
- run more tmsr benchmarks with Pronghorn


Project: multiscale neutronics coupling in the context of transients. Sn at small scale, fit into larger context. Novel materials and geometries. 


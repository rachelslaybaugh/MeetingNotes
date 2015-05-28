Workshop on Nuclear Data Need and Capabilities for Applications

Lawrence Berkeley National Lab, Berkeley, CA

May 27-29, 2015

### Meeting list
* [Day 1: 2015/05/27](#day-20150527)
* [Day 2: 2015/05/28](#day-20150528)
* [Day 3: 2015/05/29](#day-20150529)

***

### <a name="day-20150527">Day 1: 2015/05/27 

(arrived only for the afternoon session)

#### Session 2a: Energy and Other Applications

1) *Nuclear Data Needs for Understanding Material Damage*, Patrick Griffin, SNL

  - uncertainties in data are a real problem
  - list of problem isotopes  
  - dosimetry needs perspective; endf types of problems
  - fusion community needing data up to 60 MeV
  - what is IRDFF community? 

2) *Challenges and Successes in Application of the Evaluated Nuclear Data Libraries for the Missouri University Research Reactor Core Irradiation Simulations*, Nickie Peters, UM Reactor Research Center 

  - they have a very detailed model of their core, with it they can get very accurate predictions of things like critical rod positions, excess core reactivity, etc.
  - they use NJOY for xsecs
  - transport with MCNP, ORIGEN, MONTEBURNS
  - isotope production prediction with similar tools
  - they have critical rod search software that they built themselves (based on repeated MCNP KCODE calculations)
  - two publications about the isotopes where they predict specific production rates to experimental; good for many but totally off for two
  - potential mismatch issues come from not fully knowing temp of samples, so modeling of broadening is not captured
  - need to selectively pick data sets for individual isotopes


#### Session 2b: Capabilities Part 1

1) *LBNL Lab Facility Review*, Larry Phair

  - 88 inch cyclotron: 
    - high intensity light ions (protons to 55  MeV, He-3 to 170 MeV)
    - heavy ions (5 to 32 MeV/nucleon, 0.2 - 0.5 Q/M) 
  - BASE (Berkeley Accelerator Space Effects): support national security and other US space programs in the areas of radiation effects testing; protons 1-55 MeV; mimics cosmic ray damage
  - BASE also has cocktails: can get tailored thing b/c they inject multiple ions that can be injected all at one time. This allows them to extract certain frequencies. Look at LET that cause failures in things
  - a bunch of different ion sources used in these things (I am not sure if BASE is something different or goes into the 88 inch)
  - ECR is a group that does something with ion sources
  - overview of where they are and where they could go (none of this stuff means really anything to me)--however, need good shielding calculations - so it might be worthwhile for me to learn some of this stuff.

2) *LANL Facility Review*, Ronald Nelson

  - LANSCE (Los Alamos Neutron Science CEnter)
  - 800 MeV proton linac driver
  - multiple beams (H+, H-): 
    - protons (200 - 800 MeV); pRad, Blue Room, Area A
    - moderated neutrons (cold to 1 MeV); Lujan Center
    - unmoderated neutrons (0.1 to 600 MeV); Weapons Nuclear Research (WNR) facility
  - there is an ultra-cold neutron facility that is not a user facility
  - Lujan center has largely been material science, but is expanding
  - several targets are used for materials research
  - there is a proposal process for the user facility

3) *Capabilities*, Guy Savard, ANL

  - ATLAS: low energy nuclear physics national user faclity
  - stable beams at high intensity and energy (up to 10-20 MeV/u)
  - adding new capabilities (CARIBU, intensity upgrade) and expanding equipment (HELIOS, digital gammasphere and DSSD, X-array; AGFA, AIRIS, N=126 factory, laser lab, beta-delayed neutron trap)
  - CARIBU beams, heavy n-rich from Cf fission, no chemical limitations, low intensity, ATLAS beam quality, energies up to 15 MeV/u (part of ATLAS)
  - retiring their linac
  - CARIBU is their new fancy thing
  - lots of numbers about ion sources that do not mean anything to me
  - they have new techniques for beta-delayed neutron measurements
  - slide for where they are pushing for improvements (worth looking at again; slide 18)
  - applications is becoming one of the core components of the ATLAS long-range plan


#### Session 2c: Capabilities Part 2

1) *Association for Research at University Nuclear Accelerators Facilities Review*, Partha Chowdhury, Association for ... (U Mass Lowell)

  - quick run down of the facilities of the 8ish schools involved
  - deeper description of what they have at Lowell
  - talked fast; lots of info

2) *RPI Facility Review*, Yaron Danon, RPI

  - they collaborate very closely with KAPL
  - I was not paying tons of attention, but he talked about capabilities and then presented a bunch of data and examples of what they are doing


3) *ORNL Facilities Review*, Krzysztof Rykaczewski, ORNL

  - HRIBF close April 2012
  - 25 MeV tandem accelerator operated on a limited basis (cost recovery only)
  - looks like they will shut this down over the next several years and their equipment will find other homes



### <a name="day-20150528">Day 2: 2015/05/28 

#### Session 3a: National Security Part 1

1) *Needs for Neutron Reactions on Actinides*, Mark Chadwick, LANL

  - came late and did not pay attention: but lots of interest from the room about putting these things in the white paper

2) *Nuclear Data's Hidden Dysfunctia: Applications Don't Actually Depend on Structure, Do They?*, Morgan White, LANL

  - there is no relationship between the "uncertainties" on the data and how well we know the data
  - there is huge potential for large jumps in data values that get the same uncertainty assignment; we need a way to bound these things so we can have more certainty in our uncertainties
  - theory and modeling are present; nuclear structure is not included
  - there is little interaction between the communities of application and structure, this could be part of the problem
  - nuclear theory uses structure data as a black box
  - XUNDL and EXFOR should be held up for emulation
  - TINDL (from Talys code) and RIPL-3: issues with blind use or abandonment, no feedback to community to figure out what and why - only choosing what matches integral experiments
  - there are success stories of folding theory and results together to have a win
  - structure data needs to be self-consistent and complete
  - it is imperative to retread the "known" ground when it is of critical importance
  - when you need to make up numbers, you need to have the people best able to make them up do it rather than someone down the pipe who knows even less!

3) *Gamma Spectroscopic Data for Non-proliferation Applications*, Brad Sleaford, LLNL

  - 260 nuclei missing 36k gamma lines
  - IAEA + Budapest reactor combined with ENSDF -> RIPL (reaction input parameter library) + DICEBOX -> EGAF (evaluated gamma activation file) -> ENDF 
  - some back and forth on these things as they feed back
  - evaluation automation system that has dicebox as part of the system 


#### Session 3b: National Security Part 2

1) *Neutron Charged Particle Radiation Data Needs for NIF Implosion Experiments*, Charles Cerjan, LLNL

2) *NRF Applications -- An Unplanned Examination of Nuclear Data for 1-5 MeV Photons*, Brian Quiter, LBNL

  - Nuclear Resonance Fluorescence: good quick overview about this
  - photon scatter data is not ENDF ready
  - coherent = Rayleigh (still sort of studied) + Delbruck (stopped in 90s) + Nuclear Thomson + GDR (resonance?)
  - found a bug in how scattering was handled in MCNP; fixed the coherent scattering after 2011, mattered for high Z materials, esp. at high energy
  - still no photonuclear elastic scatter in ENDF database; improvement not being maintained in MCNP
  - NJOY also has bugs: cannot process non-isotropic NRF
  - photo-elastic scattering is only handled through form factors
  - MCNP has a legacy bug that is also hard-coded into NJOY: impacts coherent and incoherent scattering at large angles
  - some other applications that might be useful, but we do not really have the data yet

3) *Fission Product Yields for Neutrino Physics and Non-proliferation*, Anna Hayes-Sterbenz, LANL


#### Session 4: Medical Isotope Production




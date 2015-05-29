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

  - did not really take any notes

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

  - need to look at these slides b/c it talks about anti-neutrino spectra in reactors
  - anti-neutrino anomaly: reanalysis of conversion of aggregate beta spectrum to an anti-neutrino spectrum
  - known corrections to beta-decay are the main source of the anomaly
  - issues with forbidden transitions as a knob to turn
  - also, the "bump": around 5 MeV there is a deviation in experiment compared to prediction
  - ENDF sees the bump and JEFF does not; the two libraries have different yields (which are much larger than the evaluated uncertainties of course)
  - difference in measurements: one taken in France with a very thermal reactor (heavy water) and the others taken at PWRs with more epithermal neutrons
  - it may be that one library is closer to thermal and one closer to thermal/epi - the libraries match the experiments differently
  - information about how to use this for security: volatile fission product collection and measurement, etc.
  - they need iodine (130 and 135) measurements for forensics
  - need handful of FPs that dominate high-energy spectrum need to be measured for reactors
  - summary slide is pretty good


#### Session 4: Medical Isotope Production

1) *Nuclear Data for Medical Radionuclide Production: Present Status and Future Needs*, Syed Qaim, Research Center Julich and U of Cologne

2) *Nuclear Data, Nuclear Theory, and Isotopes*, David Dean, ORNL

  - theoretical calculations need to include error estimates!
  - slide 7 is a good overview of what goes into the calculation schemes
  - most of what goes into these are parameterizations that lots of assumptions built into them; difficult to sort all of this out
  - have we actually made progress? has changing parameters really done anything for us?

3) *Nuclear Reaction and Decay Data for Medium Energy Radionuclide Production*, Jonathan Engle, LANL

4) *Radioisotope Research and Production at Brookhaven Linac Isotope Producer*, Suzanne Smith, BNL

  - This looks like a good reference for learning about this ucop initiative
  - Pt radioisotopes appears to be a big thing
  - also a good key goals/summary slide
   

#### Session 5: Capabilities Part 3

1) *Michigan State University Facilities Review*, Sean Liddick, MSU

2) *Triangle Universities Nuclear Laboratory Facilities Review*, Werner Tornow, Duke / High Intensity Gamma-Ray Source



### <a name="day-20150529">Day 3: 2015/05/29 

NE Breakout Session:

1) William Bauder, Notre Dame
*MANTRA: A Project to Infer Neutron ...*

  - need for neutron capture data for actinides for gen-IV and advanced fuel cycles
  - MANTRA to do actinide materials in ATR (list of what they're measuring there)
  - really looking at fast spectrum, so modifying ATR's spectrum to get the spectrum that they want
  - they irradiate each sample in three spectra to compare
  - then get integral capture cross sections
  - do this with accelerator mass spectrometry (AMS): count ions
  - avoid issues with contamination, high sensitivity (10^-15 from 10^4) - keeps sample size down and keeps irradiation times short (50-100 days)
  - ATLAS facility: ion production at ECR, RFQ and PII Linac acceleration to 1MeV/u, Fragment Mass Analyzer (FMA) detector
  - challenge has been variety of isotopes they're trying to measure; they've developed a scaling program that facilitates isotope switching
  - the ECR plasma sputtering strategy leaves material on the walls around the sample that can contaminate the next source; to get rid of that they now have a laser ablation technique, which lessens contamination
  - can produce up to 1 enA of beam, peak-to-peak is unstable and they average out
  - laser minimizes cross talk compared to previous method
  - also have a multisample changer (hold 20), now done in 5 minutes per sample change; quick time helps reduce uncertainty
  - actinides separated by energy loss; strip to separate background positions, though this reduces efficiency
  - also have a Faraday cup at the focal plane to measure actual beam current
  - 4 materials looked at U-238, Np-237, Th-232, U-236 with two different spectrum filters
  - were able to keep samples fairly pure after irradiation
  - got a lot of data and could measure a large number of samples

Punchline:
  - comparing ICP-MS and AMS, they have higher precision but lower sensitivity
  - using MCNP for estimating spectra and fluence and also use U-235 flux wires to get the spectrum coming from ATR
  - after the spectrum is "correct" then any remaining discrepancies are data problems
  - adding self-shielding corrections; first analysis for these samples is not yet complete

Future:
  - AMS: continue to refine measurements and reduce uncertainty (target 5%), some comparisons

Qs:
  - after irradiation, material is prepared for analysis at INL, they do some amount of analysis first as well
  - the distinguishing feature of this method is the sensitivity and ability to use small samples irradiated for short amounts of time - this allows for measuring multiple capture xsecs
  - they have not been able to get standards for measurement; mostly getting ion source instabilities reduced so far
  - assumptions on the charge state that could cause some uncertainty; however, there is no sensitivity so things happening differently in the ECR (which is why standards would help)
  - not measuring a specific Z, measuring mass; leads to questions about unfolding intermediate steps that are inside a given mass chain
  - U-238 will be the xsec the thing they measure to make sure they get the correct value for something well known
  - flux wires kept in ATR in each run that helps ensure the flux is consistent; though the spectrum has to be unfolded
  - will not get a high-fidelity xsec, but will get a comprehensive look and that data can be folded into uncertainty analysis and some other things
  - can leverage overlapping things to get at the same data through multiple paths

2) Wesley Frey, McClellan Nuclear Research Center, UC Davis
*Facility Description and Capabilities*

  - they largely do radiography with industrial applications
  - they would like a larger research component, they have space to irradiate stuff
  - 1990 original criticality, US Air Force was original owner for F111 fwing fighter bomber to look at low-level corrosion, but then the cold war ended
  - UCD took it over for BNCT to make it the west coast source, which also did not pan out...still on McClellan air force base, which closed in 2000
  - 2 MW stead state; the core is 6 ft below grade to protect it from airplanes
  - purpose built for radiographing very large things
  - thermal flux ~3x10^5 - 4.3x10^6
  - they also do electronic radiation hardness testing for defense apps; fast neutron irradiation
  - lots of new work in defense analysis and launch stuff for NASA (heavy lift rockets)
  - research with Davis is with plant department - for diseases and issues that affect wine (basically)
  - also hydrogen fuel cell radiography
  - the upgrade to 2 MW was motivated by Si crystal doping, though that program has ended. They how run largely at 1 and 1.5 MW rather than 2 (which could be problematic for fuel integrity)
  - slide with flux #s = 11
  - also have NAA, doing some SNM irradiation for LLNL
  - ability to pulse with SNM (pulse details on slide 14)
  - 1 s xfer out of the pneumatic xfer system; ~30 minutes for sample removal out of core locations
  - MNRC has the broadest scope license in the US, so they can irradiate nearly anything
  - happy to get students involved

3) Steven Grimes, Ohio U
[1] *Comparison of Calculations of Neutron Cross Section son Deformed Nuclei Between Hauser-Feshback and Deformed Hauser-Feshbach Models*

  - Hauser-Feshbach enforces spherical symmetry, even when you're trying to model a deformed nucleus. Some ppl have used deformed level data, but that's it
  - accuracy issues associated with the presence of isospins, though that differs
  - a new formulation was made that accounts for isospin to attempt to deal with this; need to invoke isospin mixing that does some conservation and then can match experiment
  - have a mu parameter that varies between 0 and 1 where each bound leads to some limit; experiments have show 0.3-0.7 as the useful value
  - this is about an analogous situation for K (for deformation)
  - K selection rules; rules associate with J (turns decays off that are not allowed in deformed basis that would be allowed in a spherical basis)
  - this matters in our ability to calculate U
  - calculations with this new idea are n + several isotopes (Er-168, W-183, W-182, Mg-25), and alpha on Ne-22 -> does not yet do fission
  - results are ratio of spherical HF compared to deformed HF; J state impact varies by state and energy in how off the spherical case is compared to this new theory
  - continuum effects are small, but average is 20-30% change; large J resolved states are universally reduced; small J states are enhanced b/c of the degeneracy that he covers
  - there is low sensitivity to K mixing; complete K mixing does not limit to traditional HF
  - next steps are adding fission
He posits that this new model really needs to be used in evaluations and predictions; therefore EMPIRE and TALYS need these options

  - There are still errors here, but they are much less than the other model; and those errors are included in the other model so the ratio is telling
  - increases run time significantly (50-80%)
  - if you give the code the correct level density it will do the correct thing for combinations of things
  - will not do triaxially deformed nuclei

Do we need to do experiments to clarify/confirm? The best would be U or Pu, but the level states are too close together. They're trying to do Mg (?) experiments. 

[2] *Recent measurements*, just given verbally
  - 4.5 MV tandem accelerator
  - pulsed sphere experiment: drill a hole in a sphere of material you're interested in and put beam into the hole
  - Fe, measured with several energies at some outgoing angles (1, 6, 8, 10 MeV)
  - ENDF/B-VII make a model of when you should see things at detector, compare to experiment, get some information
  - demonstrated that there were significant deficiencies in Fe xsecs
  - get a pass-thru peak and a broad distribution of the scattered ns
  - n peak that came "right thru" is  most telling; if that's not correct then something is quite wrong
  - the broad distribution is more nuanced
  - for Fe got pretty good results with 1 MeV and increasing errors with higher energies. Major problems with the abs xsec
  - the broad distribution is also wrong; just fixing the absorption in ENDF didn't fix everything else
  - issues with change in flux with angle depending on sources; though they measured at many angles to try to deal with this (dd vs. dt)
  - this does not account for dd breakup, though they tried to correct for that
  - they've done Fe and would like to do some others
  - good initial investigation technique that can flag issues
  - however, you cannot distinguish between many of the exact reactions, which rxn was which; though there are useful things that you can figure out.
  - also compared to some other libraries, but they weren't right either

**Looking further at the issues in Fe and fund more pulsed spheres.**

<aside from Danon: measurements with some extra options, things still are not going well with iron>


4) Bradley Rearden, Oak Ridge National Laboratory
*Applications of Nuclear Data in the SCALE Code System*

  - 3 main projects in mod and sim: SCALE (licensing), exnihilo (HPC), nuclear data (SAMMY code; measurements to libraries)
    - SCALE V&V and UQ fed into data needs; data and SCALE modular physics go into exnihilo; high-fidelity apps from ex feed back into nuc data
    - generate continuous energy n and gamma xsecs; do problem-dependent corrections with loaded Doppler broadening - may look at on the fly in the future. Can also make multigroup n and gamma xsecs; have resonance self-shielding methods for that
    - data corrections fed back to ENDF team; really driven by application b/c they have so many real app users and they need things to be correct
  - sensitivity and uncertainty analysis: critical systems and rxn rate ratios (may be helped by MANTRA experiment); they do not yet do kinetics - depletion not transients
  - putting an adjoint version of origen together...
  - V&V is one of their initiatives that can send feedback into the data world
  - we're good at long-lived isotopes; we're not as good at short-lived isotopes (which matter in accident scenarios)
  - totally independent processing from MCNP; the only thing they have in common is ENDF
  - knowledge management slide is a good thought framer
  - need sensitivity and covariance, so can characterize how much uncertainty is introduced into your system from the uncertainties in the data
    - a clear issue is that the covariances are not good, so using it is highly suspect
    - decided to have a complete set rather than an accurate set as CSWEG; it is only okay if it does not give you a smaller uncertainty - if it gives you larger it is conservative, but it could be overly expensive. 
    - however, looking at correlations could therefore be fraught and using this for decision making may be wrong
    - assume that biases are from the data and that those uncertainties are bounded by the covariance data
  - can also use this for gap analysis - used for strategic experiment design (can try to do this better with better tools!)
  - UQ slide has good pros-cons lineup
    - continuous energy sensitivity analysis now available
    - extended to generalized perturbation theory, so now they can look at sensitivity to rxn rate ratios (this is where there could be use for MANTRA and use it for ATR analysis)
    - the UQ sensitivity info is being used pretty broadly. The data is currently adjusted to integral measurements, so it is tailored to nuc rxtrs, but that does not help lots of applications
    - some challenges are b/c it is system-specific in some ways
  - Bayesian
    - take a bunch of benchmark data values and uncertainties and apply Bayesian analysis to get rid of "computational bias" to make an unbiased set to get exact agreement with the data (does not give data for values it does not match)
    - that whole thing gives xsec update suggestions
    - U-235 nubar is good, Pu-239 nubar is overpredicted based on this stuff
    - U-238 n-gamma is not good
    - Pu-239 fission is okay...
  - they identified and fed back data issues that has been corrected
  - some issues with FP uncertainty that has used fuel implications, Eu-155 - have rankings of issues that might impact licensing; we need to know if the changes in covariance data are real or if they'll just jump around in the future; how do we deal with that for licensing?
  - gamma production data
    - many libraries don't have the data (exist in some cases but not yet evaluated, communicated) - important to HFIR
    - combined all the libraries to get as much gamma production data as possible
    - issues with negative kerma
    - (need to take these issues to CSWEG)
    - getting incorrect energy deposition as a result (franken library helped)
  - for FHR (fluoride salt-cooled high temperature reactor) has no S(alpha, beta) data for FLiBe. Do they need it? Need to push for it if it is needed. 
  
Wish List:
  - look at a wide range of applications to get a serious handle on things (can we do this in FY16 so that we have a real plan for FY17?)
  - Pu-239 nubar; U-238 n,gamma
  - Gamma production and kerma data
  - Consistent FP yield data (cumulative vs. independent inconsistency)
  - S(alpha, beta) for FLiBe


5) Krzysztof Rykaczewski, Oak Ridge National Laboratory 
*Beta-delayed neutron spectroscopy of fission fragments*

  - revival of beta-delayed neutron spectroscopy driven by several things (current data is widely inaccurate)
  - this could actually have an impact b/c some of them might be of high energy and that could actually matter
  - want beta decay strength for nuclear physics, astrophysics, etc. Sparse and inconsistent data, need standards, NE also matters
  - better ability to produce, separate, and study these now
  - also want to measure the gammas associated with those neutrons
  - r-process is really influenced by b-delayed ns
  - we have impacts on decay heat, need to use proper methods to get the whole picture
  - there is a bunch of physics we would like to understand embedded in all of these processes
  - using TOF methods and y-ray detector (VANDLE)
  - first implementation at FRIB
  - sub-nanosecond timing; system development was quite complex
  - 29 cases measured in 20 day campaign
  - VANDLE also used at CARIBU; measured 4 isotopes, calibration and some things that are complex
  - looking at effects of the shell gap to see what is that impact on the strength distribution
  - this is helping so now our models and experiments are matching much better
  - they have really demonstrated that b-delayed neutrons are high energy in decays of exotic nuclei
  - this data will go to XFOR; these are raw spectra, so that has to be accounted for
  - they did not do this with reactor needs in mind...they thought about nuclear structure
  - proposing to remeasure classic nuclei, which are important for reactors. 
  - detector is being upgraded to enhance efficiency
  - reasons for why we need VANDLE to measure some of these things (Br, I); complimenting what was measured with MTAS
  - need the $ to do it...
  - also antineutrino motivation, can capitalize on funding sources

What about doing sensitivity to these things to see if it makes a difference? 
If it does, then there is justification. 
If not, we do not need to worry about it.


#### Closing

- need to clarify what is needed for what, how that maps to funding agencies, and what the impact of improving somethiing will be
- help the agencies leverage together - may have higher likelihood of funding if they can be seen as cooperating
- foa will come out (hopefully) and will be informed by the white paper
- be specific!
- those who generate and curate the data must talk to the users and employers of the data
- we need to be more aware of the research calls that are out there
- let's get a list of facilities that we can use so we know how to leverage which things
- helpful in identifying and understanding the problems we really need to work on

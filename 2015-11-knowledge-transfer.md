INL Knowledge Transfer Workshop

Idaho Falls, ID

17-19 November, 2015

### <a name="top">Days
1. [11/17: Day 1](#day1)
2. [11/18: Day 2](#day2)
3. [11/19: Day 3](#day3)

Slides for all talks provided in associated folder.

#### <a name="day1"> Day 1

Nuclear Energy Fundamentals; George Borlodan
* neutronics
  - started in navy, licensed on 3 commercial plants, deep industry experience
  - lots of basic terms: fissile, fission, energy release, 1 eV is 10^-16 J
  - fission products are the thing that we worry about; their existence is what causes decay heat (up to 6% of rated power) that can cause accidents and produce radiation, which is the thing we don't want to be released.
  - we went through the 6 factor formula to get to k (fast fission about 3% contribution)
  - also, everything in the reactor has a male pronoun
  - how long neutrons live fast: 10^-4 s; 3-4 collisions
  - 10^-6 seconds at thermal
  - Xe-135 is about 6% of fission products (whole chain); born directly it is (not stated)
  - Noting that Xe-135 decays and Sm builds up and is only removed by neutron interaction. This is important for how they behave. 
  - methods of reactivity control: control rods (which causes local suppression and burn imbalance, which we have to think about carefully), soluble neutron 
  - 4500 MWth

* control
  - PWRs use silver, indium, cadmium in control rods
  - Navy uses halfnium in control rods
  - BWRs use boron for control rods (B4C)
  - BWRs use Gd as a burnable absorber
  - PWRs: boron is also uses for accident mitigation; we have to have boron in solution to make sure the reactor stays shut down at cold temperatures because of the excess reactivity (boric acid I think)
  - BWRs don't need soluble boron; their control rods are sufficient. They have emergency injectable boron (sodium pentaborate). They have not yet needed to use this.
  - fixed neutron absorbers: strategically place fixed poison rods or something in specific spaces for power shaping and control. These burnable rods are usually boron.
  - control rods and soluble absorber are controlled by operators
  - changing boron concentration at eol for PWRs is really hard bc the concentration is already so low - hard to lower it. Lots of water exchange and resultant waste handling. 
  - CRs used for quick operator response and protection: small power control; trip or scram (gravity in PWRs and water pressure driven in BWRs)
  - B concentration is slow control - compensates for burnup and PWR accident control
  - BWRs also use recirc control flow: controls amount of voiding (faster = less void, slower = more void)

* fluids / heat transfer
  - heat capacity: 1 BTU/F for one lbm of water; to get this to 1 lbm of steam: 1000 BTUs (latent heat of vaporization) and conversely for condensation
  - somewhere less than 100 BTUs you get water-steam mixture without temperature change
  - addition of more heat after all steam results in increased temperature but not pressure (superheat)
  - PWRs are pressurized to prevent boiling; pressure is therefore felt throughout the RCS (610 F outlet temp; 652 F at 2235 psia is saturation temp)
  - BWRs are at saturation temperature, lower pressure, high level of circulation flow
  - conduction v. convection v. radiation
  - PWR: fuel pellet -> helium gap (conduction) -> cladding (conduction) -> boundary (laminar) layer (conduction; try to diminish layer through mixing) -> bulk flow (convection)
  - PWR: forced convection transfers steam from reactor to steam generator; when pumps fail can still take advantage of natural convection caused by density differences
  - thought experiment: what if steam generator looses supply of cooling water? Will remove heat until it boils dry, fast, heat removal stops. 
  - Critical Heat Flux is when we cause departure from nucleate boiling, which hoses us. Function of temp, pressure, reactor power, flow rate
  - nucleate boiling, good for heat transfer. subcooled boiling, still good. Bubble flow ok in BWRs, try to avoid in PWRs. Slug flow, try to avoid in PWRs, still ok in BWR. Annular flow: maybe ok in BWRs. Mist flow = bad. 
  - flim dryout is the thing we care about in boilers

* Radiation principles
  - types of radiation
  - Absorbed dose: energy imparted by ionizing radiation / unit mass (rad or gray). Quality factor: accounts for biological damage. Dose equivalent is the multiplication of the two (1 Sv = 100 rem).

* LWR chemistry (might need to review these slides again
  - general corrosion can yield particles that break loose and can become crud and get activated in primary; can just gunk up secondary; pH control to prevent it; sludge lancing
  - worry about scc. PWRs this is in steam generators, BWR thing is in slide
  - good intersection slide
  - Chemistry control in PWRs: Li-OH early in life to establish basic pH. Later, B in solution becomes Li to do this, so we remove Li slowly over time by ion exchange
  - de-oxygenation to prevent corrosion by adding H2 - it recombines with O under the strong radiation environment. added as a gas in chem and vol control system vol control tank. Also have to worry about degassing. Add N to get the H out and burp it.
  - specific chemicals are added, like Zn, for specific scc prevention
  - for secondary most PWRs use all volatile treatment (AVT): hydrazine removes O at lower temp and transforms to ammonium at higher temp to raise pH
  - also, BWR notes. There is a bigger dose rate and release issue because of the single loop. Competing things, H2 helps prevent SCC but increases N-16 dose rates. They add a delay line to help reduce the gamma impact of N-17
  - BWRs use H water chemistry to reduce SCC; noble metal chemical addition to reduce H (Pt and Rh); condensate polishing to reduce Fe; Zn to reduce dose rates and SCC

* Process temperature measurement
  - Temperature. most common: resistance temperature detector (resistance changes as a function of temp; use something with linear change; we use Pt; wheatstone bridge is method of measurement. good: stable; bad: limited in range, esp in up temp) and thermocouple (two dissimilar metals [Al, Fe] generate a potential [Thompson effect] when exposed to temperature change. good: higher temp range)
  - Pressure. Bellows: pressure felt on one side vs. another (diaphragm). Another one where a bar pushing in one direction is felt, a current is used to counter the force, and that is what gives the measurement (the thing itself holds still). How these behave and perform change under adverse environmental conditions; that uncertainty has to be characterized and accounted for.
  - Level. Differential pressure transmitter, usually a bellows, that measures a column of water. Use a wet and dry reference leg. 

* Components
  - Pumps. Net positive suction head (diff between P on the suction side and the saturation P on of the fluid); It prevents cavitation. Pump Shutoff head. Gas Binding. 
  - Valves. Gate valves; the packing is really important. Globe valve; pretty simple, it can make some headloss, but is quick acting and can be used for throttling. Butterfly, also simple, can turn into flow stream. Ball valve, pretty simple and minimal pressure drop when fully open. Diaphragm valve a little more complicated, but eliminates packing leakage compared to a gate. Check valve, allows flow to move in one direction. Relieve or Safety; when pressure on unpressurized side goes high enough lets out; potential issue with difference between start to open and full open (accumulation); blowdown is how far below setpoint that valve fully closes (e.g. 100/110/95). 
  - Valve operators. handwheels. motor operated valves (usually gate or globe or butterfly; these can be really complicated and are prone to many types of issues). Air (diaphragm); consider air to open or air to close as an important choice. Solenoid (globe valve); Target Rock PORV has had lots of failure modes: control circuit failures, binding, liquid phase issues, thermal expansion problems.
  - Valve terms: bonnet: mates with the body of the valve and supports the stem, disk, and valve actuator. Disk controls the flow. 
  - Motor terms: AC induction motor: uses a series of conductors (must be ac), the 3 phases rotate, induces magnetic field, rotor follows. Slip is the difference between the stator rotating field speed and the rotor. Starting current can be 6x the full load operating current. Synchronous motor: rotor field is created externally, rotor speed = stator rotating field. Locked rotor: too much load cases rotor to stop and current just goes up (on induction motor). 
  - Generator terms: true power: power consumed by the resistive loads in an electrical circuit [W]; reactive power, power consumed in the AC circuit because of the expansion and contraction of the magnetic and electrostatic fields (fake, but measurable. does not require work, but wires need to be able to carry it) [VAR]. Power Factor: difference between true and apparent. Apparent is voltage and current (hypotenuse). Paralleling: get voltage and frequency to be aligned to connect a generator to an AC circuit. 
  - 

Selected LWR Plant System Overview; George Borlodan


Fukushima Daiichi Accident Video


Nuclear Safety Design Overview; George Borlodan


Regulation and Industry Groups; George Borlodan

 
[Index](#top)



#### <a name="day2"> Day 2

 
[Index](#top)



#### <a name="day3"> Day 3

 
[Index](#top)


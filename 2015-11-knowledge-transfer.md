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
  - how long neutrons live fast: 10^-4 s; 3-4 collisions
  - 10^-6 seconds at thermal
  - methods of reactivity control: control rods (which causes local suppression and burn imbalance, which we have to think about carefully), soluble absorber 
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
  - PWR: forced convection transfers steam from reactor to steam generator; when pumps fail can still take advantage of natural convection caused by density differences
  - thought experiment: what if steam generator looses supply of cooling water? Will remove heat until it boils dry, fast, heat removal stops. 

* Radiation principles

* LWR chemistry (might need to review these slides again
  - general corrosion can yield particles that break loose and can become crud and get activated in primary; can just gunk up secondary; pH control to prevent it; sludge lancing
  - worry about scc. PWRs this is in steam generators, BWR thing is in slide
  - good intersection slide
  - Chemistry control in PWRs: Li-OH early in life to establish basic pH. Later, B in solution becomes Li to do this, so we remove Li slowly over time by ion exchange
  - De-oxygenation to prevent corrosion by adding H2 - it recombines with O under the strong radiation environment. Added as a gas in chem and vol control system vol control tank. Also have to worry about degassing. Add N to get the H out and burp it.
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
   


Fukushima Daiichi Accident Video part 1


Selected LWR Plant System Overview; George Borlodan
- explanation of systems on PWRs. regenerative heat exchanger is a crud trap. Drew some things on diagram
- lots of info about flow rates and things not on the picture that I did not catch all of.
- Westinghouse SGs are above to take advantage of gravity and natural circulation. Note: only one pressurizer on 4 loops. 
- BWR the hot leg goes way up (candy cane) then thru straight pipes, 2 cold legs and 2 pumps come out of the bottom. This design gets superheated b/c the cooler steam from the bottom goes up and passes the hotter water and gets a boost. However, no inventory in the SG. 
- something about J tubes to prevent water hammer and NRC arguing about whether or not they were safety related. 
- exit of swirl vanes, 80-90% quality; then chevron separators keeps the water from making the zig-zag turns. 
- fuel rods do not touch bottom or top nozzle. The springs hold them in and they can expand in either direction.
- PWR Tav = 547 F with no load, 577 F at full load (forced Tav) because of the steam pressure.
- in a PWR you control the turbine to change power: more power takes more steam from steam generator, which makes more cold water enter reactor, which adds positive reactivity, increasing power. This relies on negative moderator temp coeff. They pick up real power from the grid to do this. The operator then has to change reactivity control to keep Tav at the right place. 
- PWR containment is designed for complete evacuation of the primary system (double-ended guilliotine) BWR containment is small and designed for a full break of a recirc line and emptying of reactor. 
- no atmospheric release valves on BWR to keep radiation inside - instead discharge them through suppression pools to filter; spargers to remove heat. 
- BWR recirc strategy is to keep average water level higher to prevent dryout.
- Water used in hydraulic cr working is the same as the condensate water so it's okay if it leaks. 
- on BWR startup no recirc flow to let things heat up. To cooldown do steam dump to the condenser, residual heat removal when low pressure.
- in a BWR power control is by pump speed. Reactivity control is done with control rods. To increase power, increase flow, this causes increased reactor power because there's less voiding. This heats up, more steam, control valves open more, more torque on generator = more electricity (turbine at constant speed). You set reactor power at what you think will make the right kW amount, and the controls follow (PWR is reversed). 


Nuclear Safety Design Overview; George Borlodan
- 3 safety functions: keep core controlled, keep core cool, keep core contained, 
- containment for Hinkley C: 150 pounds. Yeah, these things are expensive.
- went to notes on paper...

[Index](#top)



#### <a name="day2"> Day 2

Regulation and Industry Groups; George Borlodan
- Title 10 of CFR in the US is very large. In the UK the rules are implicit, in US they're explicit. 
- made a leak-proof containment for reactors near large population centers: NY and Chicago; pretty cool technology
- Appendix A: general design criteria (could be useful in this startup think-through thing). 
- Appendix B: Quality Assurance Criteria (again, a thing that will be useful for this).
- INPO: owned and operated by utilities. Promotes best practices, guidelines, etc. 4 cornerstones. 
- WANO and INPO have strong communication, but are separate. WANO started after Chernobyl


-----------------------------------------------------------
Introduction; Phil Hildebrandt
- Hi to Per
- Naval vessels are weapons delivery platforms that happen to be propelled by reactors; they're not plants.
- We started with the navy, but the needs are totally different (e.g. people live on these, so we have to make different kinds of choices - can't do BWRs, for example). 
- each plant has it's own personality. 
- L->R TMI unit 2 on right, the one with an accident. Unit 1 and 2 are different plants, designed by different companies. Involvement in the design of 1 was more involved than 2. Totally different personalities. Davis Bessie, B&W, but a different plant that's in northwest Ohio; different cultures in different locations. La Salle, BWR, misoperated by management. DC Cooke, ice condenser plant that was an Achilles heel.
- Think about how all of these things affect what we do. Transfer knowledge to the next generation of leaders (it seems a little random that I'm here).
- slide 6: in recent years, operators, maintenance, and owning companies engineers are starting to have more input into design and regulation choices. How is something going to be used in the field. Dedicated commercial grade: I have a design need, only source is commercial, I have to demonstrate that it is ok to use that.  


Role of Management; Phil Hildebrandt
- management is woven into the tapestry of everything that happens; no excuses, but management crafts the context in which things happen
- I like slide 3. Tension between science and operation. 
- Direct conflict of view of who was responsible for safety: owner thinks reg, reg thinks owner, operator views owner trumps regulator
- We oversold how easy nuclear was going to be - so some utilities got into the industry that should not have; they weren't prepared to take on the challenge beyond just operating large fossil plants.
- New view has corrected some of these flaws. Part of why PAAA makes sense is because the utilities don't actually own the fuel, they manage it. PAAA is an insurance policy, not a liability statement. We get to view it that way in part because of this fuel ownership issue. License holder, however, is civilly and criminally responsible for licensed activities.
- The regulator needs to be the owners best friend
- note: 1970s perspectives tend to come up and be present still today in some instances and locations; pressure to adopt current views
- slide 8: operators made decisions based on what they believed their management's expectations were. Things that were really emphasized colored their decisions that ended up leading to accidents or near accidents. 
- Keep management aware about the consequences in terms of the technology of compromises that need to be made for schedule and cost 

- real barriers to advanced technologies: economics. Historically, momentum. Today, looking at big companies, mpower, couldn't get equity; NuScale will need equity soon; TerraPower, same deal. To take these to success, it will take a very strong signal from future owners otherwise these companies will never be able to get the equity. Clear signals to wall street, the developer, and the regulator. Can get to technical agreements, but need to translate those agreements into policy issues that were created in the 60s. Those discussions are conducted in public and all anti-nukes get input into that process. You have to undo the policy choices in the public arena. This is why you really need a strong hand (also, a shift in the public). DOE pounding on the table is irrelevant - they won't buy or license any of this. They are a false stakeholder. 
- What's the government role in this? Gov needs to be highly involved, and the current investment is not nearly enough. 


Nuclear Plant Accidents; Roger Mattson
* Three Mile Island Unit 2
  - they weren't sure if rcs pumps would start b/c there was a capacitor that was sensitive to radiation, they therefore couldn't turn the one running off
  - H explosion: localized near dump tank, so pressure of explosion wouldn't have been uniform on containment; rated to 60 psi (is the design pressure, not the pressure at which it will fail), chart recorded 28, likely higher.
  - leaking radioactivity expected to get worse, NRC recommended to evacuate, there was hesitation, leak stopped so that was fine (I lost track of who was whom here, but that all looked bad).
  - There were several precursor items: culture - warnings about Davis Besse was let slide, someone had thought through issues with the candycane steam generators and said no it will be fine. Lots of missed chances. [complacency and mindsets]
  - Phil: perspectives: [1] regulator who should be regulating is helping to solve the problem instead so no one is verifying that work; industry was not well-prepared; the NRC was in the midst of this accident, which was totally inappropriate. [2] Davis Besse: PORV thing that was the same as at TMI. B&W understood that incident well, they messed up by not telling anyone else what happened at 1977. [3] philosophy that regulator is responsible for safety rather than the owner, which is who is really responsible. 

* Chernobyl: this was really and truly a tragedy on many levels. 
  - book: A Blaze

* Fukushima Dai-ichi units 1-4
  - root cause: lack of questioning of authority and orders is a very deep part of the culture. This percolates through entire system. 

- Note: FLEX is not the solution, it is the belt+suspenders backfit plan. 


Cybersecurity lunch talk


Safety Case; Bob Brodsky, Bob Youngblood, Phil Hildebrandt, Greg Gibbs
* Bob B: introduction

* Bob Y: evolution of safety basis - basically the history of PRA

* Phil: defense-in-depth

* Phil: shortfalls in regulatory requirements

* Phil and Greg: operating experience

Design; Henry Stone, Robert Brodsky, Phil Hildebrandt, Herb Estrada
 
[Index](#top)



#### <a name="day3"> Day 3

Design; Henry Stone, Robert Brodsky, Phil Hildebrandt, Herb Estrada
- serendipity does not count as defense in depth
- the problem at Davis Besse when they had this cross line backup plan thing that was an issue, they ultimately solved the problem by adding diversity of pumps; they did this because it was a backfit and it was a complex problem. They would have done it totally differently if they had planned from the start.
- Browns Ferry fire wiring things required addition of all kinds of things, which ended up being very expensive for the industry. Appendix R. This required increased staff to go deal with things in case there's a fire in the control room. Big requirements about separation in the cable spreading room so that one fire can't take everything out. Need a 20ft separation, a remote shutdown panel, and up to a 3 hour fire barrier between paths. 
- Lots of issues with not doing sufficient testing at scale or in the appropriate conditions. This ends up being really expensive and potentially unsafe. Really tough to get all of these things fully vetted and thought through. 
- How do we make sure that DOE participates by building the test and support facilities really needed to support nuclear? NRC isn't going to build the stuff that industry needs for testing; industry can't afford to build the stuff that it needs for testing. This is the real role of DOE. It's good that all of these agencies are separated, but we need to ensure strategic coordination to make sure that real issues get addressed. 
- Slide 36 is really good. New designs need:
  - Intrinsic Safety
  - Simple, robust design
  - Impervious to direct and consequential effects of external events
  - Operator action not required to mitigate accidents, nor can they cause or worsen accidents
  - No off-site impacts (public safety, environmental, or economic) of severe accidents [is this a realistic thing to attempt to achieve? Is it even possible?]
- Historically, the approach to design has been to fix issues, not to start with a simple approach.


Licensed Operations; George Borlodan
- Accidents happen fast. Alarms go off and things trip, they're just figuring out at all what's going on - get the procedure out, check that this thing is off, then just start figuring out what information they have. 
- Davis Besse 1977: an indication came in that made them say "close the porv block valve just in case" and that fixed it; 20 minutes into event - basically was just to try something. They didn't even know what they did. 
- Transferring from navy vessels to commercial isn't as straightforward as they may have thought - things really were different. 
- Development of systematic training taken from army model: Analysis Design Development Implementation Evaluation is how you build your training program. Think carefully about what needs to be known and all of the steps (A), how will it best be taught (D), develop the tools for teaching it (D), teach it (I), and figure out if they learned it (E). Refine as necessary. This approach is part of INPO training accreditation. Also part of 10 CFR 50 and 55.
- Personnel challenge in France during outages: they can only work 60 hour weeks and are limited to 12 hour days.  
- In the 90s shift from focus at all levels of the organization from implementing high safety standards to justifying minimum safety standards. All driven by economics.
- 90s: slide 26 is good. 
- Fukushima operator lessons are about training for extreme events and thinking about how to provide support for emotional impacts in extreme events.
- passive: let's call it nature-powered safety
- "A computer is only as good as the human who programmed it".
- The role of the operator must be clearly understood throughout all parts of the design process. Need Systematic Approach to Training based on control room tasks. Professionalism.  


Fukushima Daiichi Accident Video part 2
- Keep cognizant of the impacts of Fukushima and Chernobyl. It is important to really keep this close to my thinking when thinking about nuclear.


Human-Machine Interface; Herb Estrada, George Borlodan
- focus on the complexity of the Rankine cycle and all of the things that operators have to think about.
- it is important to design this well, and it is also hard.


Testing and Surveillance; Phil Hildebrandt
- Need to understand what you are actually trying to test
- Need to monitor what you think you are monitoring
- Need to incorporate lessons learned into testing and surveillance


Economics; Greg Gibbs
- Read through these materials, we went sorta fast and my eyes were already starting to cross (4pm of 3rd day).
- IMPORTANT: Shannon about uses of nuclear in combo with renewables to have them all be on all the time: uses for excess electricity, heat, something to capitalize on this. 


Closing; Phil Hildebrandt
- send comments; specifically about doing this for faculty. 


[Index](#top)


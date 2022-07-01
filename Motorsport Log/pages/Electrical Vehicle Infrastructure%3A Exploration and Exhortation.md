title:: Electrical Vehicle Infrastructure: Exploration and Exhortation
speaker:: Prof. R.K. Singh, Department of Electrical Engineering, Indian Institute of Technology (BHU)
date:: [[Jun 22nd, 2022]]
venue:: G-34/ Google meet
attended_by:: [[Sai]]

- #+BEGIN_WARNING
  This page is yet to be completed
  #+END_WARNING
- ![Notes for lecture on EV.pdf](../assets/Notes_for_lecture_on_EV_1656699832878_0.pdf) by [[Sai]]
- # Power Electronics
  collapsed:: true
	- Power Processors - Technology that regulates, processes and stabilizes input electricity
	- Modern loads are very high
	- Power electronics & EV are the next big thing
- # EV Charging Infrastructure
  collapsed:: true
	- Wired, wireless, private, public, battery, offgrid, OCPI Protocol
	- Common Standard - Open Charge Point
	- Location is important
	- Connectors -
- # Types of Chargers
  collapsed:: true
	- Chargers have to be universal
	- AC vs DC
	  collapsed:: true
		- AC - Level 2, LevelLV11
		  collapsed:: true
			- Onboard charging system required in the car
		- DC Charger
		  collapsed:: true
			- Charger connected directly to battery
			- Rapid charger - Level 3 fastest
			- Types
			  collapsed:: true
				- SAE
				- CCS - can use all 3 levels at some extent
				- Chaedemo
				- Tesla - Super charger
				  collapsed:: true
					- unique, but closed (not open source design)
	- Onboard vs  Offboard
	  collapsed:: true
		- Onboard
		  collapsed:: true
			- Rectifiers
			- Some addition to the cost
	-
- # Types of Connectors/Interface
  collapsed:: true
	- AC Level 1 $\to$ AC Plug
	  collapsed:: true
		- If PEVs come with LV11 cordset, no additional equipment
	- Standard
	  collapsed:: true
		- Nemo connector & SAE J1772 connector
		- 8 hrs at 120v can provide 40miles of charging
	- Slow Level 1
	  collapsed:: true
		- Common chargers
		- Car will charge in 8-12 hrs
		- 3-6KW
		- Tethered/Untethered cables
	- Level 2 Fast Charging
	  collapsed:: true
		- 80A/19.2KW
		- Residential operate at low conditions 30A, 7.2 KW
	- Level 3
	  collapsed:: true
		- 72KW, 22KW
- # Significance of Pins in Conductor
  collapsed:: true
	- Large, control, proximity pins
	  collapsed:: true
		- Large - Power transmission
		- Control - Controls charging current, by sensing PWM signal
		- Proximity - Ensure connectivity
	- another control pilot can be used to command vehicle to reduce max charging current
- # Types of Connectors
  collapsed:: true
	- |Charging Level|Type|Feature|
	  |--|--|--|
	  |1|AC|1 Phase|
	  |2|AC|3 Phase|
	  |3|DC|3 power & 7 signal pins <br />Chademo|
- # Battery Swapping
  collapsed:: true
	- Exchange your batteries at energy operator outlet
	- only possible for lower power rating
	- SOH - Day by day decreasing
	- Battery Specification for different EV segments
	- Battery Management System
- # Evolution of Batteries
  collapsed:: true
	- Lead-Acid
	- Nickel Cadmium
	- Nickel Metal Hydroxide
	- Lithium-ion
	  collapsed:: true
		- Best choice yet
- # BMS
  collapsed:: true
	- Battery Management System
	- Types
	  collapsed:: true
		- Topology
		- Distributed - Master Controller
		- Modular - Master-Slave
		- Centralized - Central
	- Operation
	  collapsed:: true
		- Monitors, Cells, Voltage, Battery Pack
		- Uses master disconnect
	- State of charge
	  collapsed:: true
		- Battery Capacity = $\frac{\text{Remaining Capacity}}{\text{Total Capacity}}$
		- Coulomb Counting
		  collapsed:: true
			- Charging current is measured and integrated over time to find energy in battery
	- State of Health = $\frac{\text{Total Current Capacity}}{\text{Total Beginning Capacity}}$
	  collapsed:: true
		- The total battery capacity of any battery degrades over time
	- Over/Under Temperature Protection
	- Charging/Discharge Protection
	- Overcurrent Protection
- # Cell Balancing
  collapsed:: true
	- > Battery balancing and battery redistribution refer to techniques that improve the available capacity of a battery pack with multiple cells and increase each cell's longevity.
	- ## Types
	  collapsed:: true
		- Passive
		  collapsed:: true
			- Burns excess charge using dummy load
			- turns on MOSFET for cell whose voltage is higher
		- Active
		  collapsed:: true
			- Eg: Capacitor/Inductor/Remote cell connection
		- Lossless
		  collapsed:: true
			- Reducess losse and complexity
			- high voltage cell will be removed
- # Environmental and mechanical concerns
  collapsed:: true
	- (ingress protection? huh?)
	- to protect against liquid/solid particles
	- IP ratings
	- EV protocols in charging
- # Conventional EV Charger
  collapsed:: true
	- Vanilla charger
	- Severe ripples, reduces efficiency
- # Miscelaneous
  collapsed:: true
	- CCS Combo 1 & 2
	  collapsed:: true
		- PLC - PowerLine Communication
	- Retrofitting is a problem
	- Wireless Charging Interface
	- Inductive Charging - Level 2 Operation
	- Renewable Based Mix Energy System
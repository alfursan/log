tags:: Calculations
by:: [[Azhar]]
verified:: [[Thahir]]

- ## Terms
	- | Symbol              | Meaning                                 |
	  | ------------------- | --------------------------------------- |
	  | $W$                 | Car Weight                              |
	  | $l$                 | Length                                  |
	  | $\mu_{T}$           | Coefficient of Friction (road and tire) |
	  | $\mu_{\text{pad}}$  | Coefficient of Friction of Pad          |
	  | COG                 | Center of Gravity                       |
	  | $b$                 | Brake Bias                              |
	  | $PR$                | Pedal Ratio                             |
	  | $r_\text{rotor}$    | Rotor Radius                            |
	  | $r$                 | Tire Radius                             |
	  | $\tau_{ F }$        | Torque in front                         |
	  | $\tau_{ \rm{PFW} }$ | Torque per front wheel                  |
	  | $\rm{MC}$           | Master Cylinder                         |
	  | $D_P$               | Piston Diameter                         |
	  | $N_P$               | Number of Pistons                       |
	  | $A_P$               | Piston Area                             |
	  | $F_D$               | Force on Driver                         |
	  | $P_f$               | Pressure in front                       |
- ## Front
	- ### Assumptions
		- $W = 250 \rm{kg} = 550 \rm{lb}$
		- $G_x = 1.6g$
		- $\mu = 1.6$
		- COG(h) $= 320\rm{mm} = 12.6\rm{in}$
		- $l = 2300\rm{mm}=90.5\rm{in}$
		- $b = 0.5$
		- PR $= 2.48$
		- $r_\text{rotor} = 5 \rm{in}$
	- #### Total Weight Transfer in $X$ direction
		- $W_{\rm{tf}} = \Delta W_x + \frac{W}{2}$
			- $55.652 + \frac{250}{2}$
			- $180.652 \rm{\ kg} = 247.51933 \rm{\ lbf}$
	- #### Front when locking torque required
		- $r = 10\rm{\ in} = 254\rm{\ mm} = 0.254\rm{\ m}$
		- $\tau_{F} = r \times W_{\rm{tf}} \times \mu_{T}$
			- $0.254 \times 180.652 \times 1.6$
			- $73.4169 \rm{\ Nm} = 3960.309 \rm{\ lb \ in}$
		- $\tau_{ \rm{PFW} } = \frac{ F  }{2}$
			- $\dfrac{3960.309}{2} \rm{\ lb \ in}$
			- $1980.1546 \rm{\ lb \ in}$
	- ### Master Cylinder an Piston
		- $\rm{MC}_\text{bore} = 0.625 \rm{\ in}$
		- $\rm{MC}_\text{area} = \frac{ \pi \times ( \rm{MC}_\text{bore} )^2 }{4}$
			- $0.31 \rm{\ in}^2$
		- $D_P = 0.98 \rm{\ in}$
		- $N_P = 4$ per caliper
		- $A_P = \frac{ \pi \times {D_P}^2 }{4} \times N$
			- $30.04 \rm{\ in}^2$
	- ### Force Required by driver to lock wheels
		- $$
		  F_D =
		  \frac{
		  \left[
		    \frac
		    {
		  	  \left(
		      \frac{\tau_F}{ MC_{\text{bore}} }
		      \right)
		    }
		    {
		      2 \times r_\text{rotor} \times \mu_{\text{pad}} \times A_P
		    }
		  \right]
		  }
		  {
		  	PR \times b
		  }
		  $$
		- $$
		  \frac{
		    \left[
		      \frac
		      {
		    	  \left(
		        \frac{1980.1546}{ 0.625 }
		        \right)
		      }
		      {
		        2 \times r_\text{rotor} \times 0.42 \times 3.04
		      }
		    \right]
		  }
		  {
		    	2.48 \times 0.5
		  }
		  $$
		- | 5in Rotor           | 8in Rotor           |
		  | ------------------- | ------------------- |
		  | $307.693 \rm{\ lb}$ | $192.308 \rm{\ lb}$ |
	- ### Line Pressure
		- $P_f = \dfrac{ F_d \times PR \times b}{ MC_\text{arm} }$
			- $\dfrac{192.308 \times 2.48 \times 0.5}{0.31}$
			- $769.232 \rm{\ psi}$
	- Specs
		- Calipers
			- ISR-22-048 (front wheels)
			- ISR-22-049 (rear)
		- Tilton 78 (Pivoting Type)
			- 5/8" front (bore)
			- 1" rear (bore)
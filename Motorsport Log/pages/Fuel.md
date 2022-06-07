tags:: Calculations
by:: [[Azhar]]
verified:: [[Thahir]]

- ```calc
  distance = 22
  bikeWeight = 250
  carWeightIgnoringAir = 370
  carWeight = 400
  
  bikeFuelConsumptionRate = 4.9
  perWeight = carWeight/bikeWeight * 100
  carFuelConsumptionRate = perWeight * bikeFuelConsumptionRate/100
  carFuelConsumptionRatePerKm = carFuelConsumptionRate/100
  carFuelConsumption = carFuelConsumptionRatePerKm * distance
  ```
	- Fuel Consumption Rate $\frac{L}{100km}$
	- Distance $km$
- Problems
	- we did not take into account the effect of increased drag
	- Thahir got confirmation from Azhar that it's okay to be neglected currently
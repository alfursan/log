tags:: Calculations
by:: [[Azhar]]
verified:: [[Thahir]]

- ```calc
  cr = 13.5/1
  k = 1.4
  
  eta = 1 - ( 1/ cr^(k-1) )
  
  bikeWeight= 250
  carWeightIgnoringAir = 370
  carWeight = 400
  
  bikePower = 73.5
  carPower = 70
  
  pwrBike = bikePower/bikeWeight
  pwrCar = carPower/carWeight
  
  fractional = pwrCar/pwrBike * 100
  loss = (pwrCar-pwrBike)/pwrBike * 100
  ```
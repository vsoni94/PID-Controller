# CarND-PID-Control
   
## Details of implementation
PID has been implemented in 'PID.cpp'. Function 'UpdateError' calculates integral, proportional and derivative errors and 'TotalError' calculates the total error using Ki, Kp and Kd respectively 

## Effect of P, I and D components
### Proportional

Proportional control tries to steer the car towards the center but it overshoots very easily and vehicle goes out of the road. 

### Derivative

Derivative control is helpful in countering the overshoot because of proportional control.

### Integral

Integral control is used to eliminate bias but it can make the car go in circles, if used alone.

## Selection of Hyperparameters
The values of Kp, Kd and Ki were selected by trial and error.

1. First, I made sure that the car can drive straight with all the parameters as zero
2. Then, I added proportional control so that the car starts to follow the road
3. Then, differential control was added to prevent overshooting
4. Integral component was resulting in the car to go out of road. So, it was kept at zero.

## Results

The car was able to drive along the road without any issues.
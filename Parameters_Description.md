# Introduction
In this file, you can find explanation about the PID parameters effect, and how I selected these values.

# Error Parameters
## Kp
Kp is the proportional error parameter. Having this parameter will steer the car when the CTE is high. If this error is large, the car will overshoot and will oscillate around the correct line. If it is low, then the car will not steer enough making it crashes into the roud edges.

## Ki
Ki is the integral error parameter. Having this parameter will ensure that the car will converge exactly on the correct line, not far from it. Having this value high will cause the car over shoot. Having it low will not help the car converge near the center.

## Kd
Kd is the derivative error parameter. Having this parameter will reduce the over shooting effect, and reduce the oscillating after convergence. 

# How I set the paramters?
* I tested intially with Kp. the car kept oscillating around the center. 
* I reduced Kp and added some Kd. The car converged near the center, but sometimes it did not steer enough at the turns.
* I increased Ki a little to ensure convergence at the center, and increased Kp to ensure that the car will steer enough. Also increased Kd to ensure that the increase in Kp will not make the car over shoot.

The final parameters are : Kp: 0.12, Ki: 0.0001, Kd: 1.0.

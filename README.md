# Pendulum-with-Spring-Animation

# Pendulum with Spring Animation

This Python script provides a simulation of a two-mass system connected by a spring and set in pendulum motion. The script utilizes `numpy` for numerical operations, `scipy.integrate` to solve the system of equations governing the motion, and `matplotlib.animation` to animate the results.

## Code Description

The script sets the physical parameters for the simulation: the gravitational acceleration `g`, the length of the pendulum `L`, the spring constant `k`, and the two masses `m1` and `m2`. 

A function `der_state` is defined to compute the derivative of the given state. This function represents the differential equations of motion for the system. 

The time span for the simulation is set, and the time-dependent solution to the equations of motion is computed using the `scipy.integrate.solve_ivp` function, with the `der_state` function as the system of equations. 

The script then transforms the angular position solution to Cartesian coordinates. This will be used for the animation.

Finally, an animation of the system is created using `matplotlib.animation.FuncAnimation`. In this animation, the pendulum is shown swinging under gravity and the influence of the spring force. The two masses oscillate due to the spring, and the spring's length changes according to the relative motion of the two masses.


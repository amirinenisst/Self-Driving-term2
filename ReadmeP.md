# PID Controller
Udacity SDCND Term 2, Project 4

## PID controller Basics
PID control is a feedback control technique that controls cross tract error(cte) by combining proportional term, integral term and derivative term.
cte is the error abserved between desired state and observed state.
* Proportinal(P) term takes the present value of cte to steer the vehicle in desired direction. P term leads to overshoot.
* Integral(I) term considers the cte over the past time. I term particularly resolves the drift around turns.
* Derivative(D) term considers the rate of change of cte to reduce the overshoot and dumped oscillations.

# Tuning
I used manual tuning through trail and error. A large proportional gain implies a large change in the output for a given change in the cte. If the proportional gain is too high, the vehicle becomes unstable. In contrast, a small gain results in a small output response to a large input error, and therefore less responsive controller. If the proportional gain is too low, the control action may be too small when responding to disturbances. While trying to balance I choose 0.2 as the P-term coefficient.
The integral term accelerates the movement of the process towards set state and eliminates the residual steady-state error that occurs with a pure proportional controller. The proportional controller causes lots of overshoot which can be reduced by derivative term and its the slope of the cte.Manual tuning is a lot of tedious work and at last I choose 0.2, 0.0042 and 3.02 and vehicle worked well on the road.
These parameters work well for this part of application but will fail to react to changes in the environment and mechanical failures of the car.


## Building
The main program can be built and run by doing the following from the project top directory.
```
mkdir build
cd build
cmake ..
make
./pid
```

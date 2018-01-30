# PID Controller
Udacity SDCND Term 2, Project 4

## PID controller Basics
PID control is a feedback control technique that controls cross tract error(cte) by combining proportional term, integral term and derivative term.
cte is the error abserved between desired state and observed state.
* Proportinal(P) term takes the present value of cte to steer the vehicle in desired direction. P term leads to overshoot.
* Integral(I) term considers the cte over the past time. I term particularly resolves the drift around turns.
* Derivative(D) term considers the rate of change of cte to reduce the overshoot and dumped oscillations.

# Tuning
I used manual tuning through trail and error. Manual tuning is a lot of tedious work and at last I choose 0.2, 0.0042 and 3.02 worked well.

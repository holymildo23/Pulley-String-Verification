# Tension-Distribution

Experimental and computational verification for the General Physics group project based on the paper **"Force and torque of a string on a pulley"** by de Oliveira and Lemos.



## Project Description

This repository contains the experimental data, computational code, and figures used for the verification part of the project.
The project compares analytical predictions with experimental measurements and visualizes the tension distribution and non-slipping condition of a string-pulley system.


## Experimental Data

The experiment was performed using a string-driven rotating disk system.

Two driving mass cases were tested:
- 1 coin
- 2 coins

For each case, six trials were recorded. The measured values include:
- Falling distance h
- Falling time t
- Angular displacement Δθ
- Average angular speed ω_avg

The experimental results are stored in:
- experimental_data.csv

The mean angular speeds were approximately:
- 1 coin: 14.68 degree/s
- 2 coins: 28.38 degree/s

This shows that the two-coin case generally produced a larger average angular speed than the one-coin case.


## Main Equations

Approximate torque:
τ ≈ R m_d g

Average angular speed:
ω_avg = Δθ / t

Capstan equation:
dT/dθ = μT
T(θ) = T₁e^(μθ)

Non-slipping condition:
T₂ / T₁ = e^(μπ)
M > 4m₁(e^(μπ) - 1)


## Files

- experimental_data.csv : experimental measurements for one-coin and two-coin trials
- tension_distribution.ipynb : Jupyter Notebook for the Capstan equation and tension distribution simulation
- non_slipping_condition.ipynb : Jupyter Notebook for the parameter-space analysis of the non-slipping condition
- experimental_angular_speed_graph.png : graph comparing average angular speed for one-coin and two-coin cases
- tension_distribution_graph.png : graph of theoretical and experimental tension distribution
- non_slipping_condition_graph.png : 3D graph of the critical pulley mass condition

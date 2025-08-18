---
layout: default
title: Wind Estimation
permalink: /wind_estimation/
---
# Wind Estimation
*Provably effective wind estimation for safe and reliable flight*  

## Overview  
Knowledge of wind velocity is fundamental across fields ranging from atmospheric science to aeronautics. Accurate wind information supports critical applications such as weather forecasting, flight safety, and efficient path planning. For aircraft, measurements of airspeed, angle of attack, and sideslip angle depend on reliable wind data, enabling both pilot decision-making and advanced automation.  

Direct wind measurements, however, are often constrained by cost, payload, or operational limitations. Traditional sensors such as anemometers and multi-hole probes may not be feasible for small unmanned aerial vehicles (UAVs) or may fail in regions of flight with insufficient airflow. To address these challenges, our research develops **estimation techniques that infer wind velocity indirectly from aircraft motion**, eliminating the need for specialized sensors. These methods apply across a broad spectrum of vehicles, from small UAVs to large commercial aircraft.  

## Approach  
Wind estimation is challenging because it is inherently a **nonlinear problem**. Standard filtering techniques, such as the extended Kalman filter, provide only local guarantees and can break down during aggressive maneuvers or in rapidly changing wind conditions — situations common in urban air mobility scenarios.  

Our approach is to design **nonlinear observers** that provide stronger mathematical guarantees: instead of relying on approximations, these observers ensure stability and convergence of the estimation error dynamics. Two main approaches have been developed to accomplish this task.
1. **Symmetry-preserving reduced-order wind observers**  
   - Motivating application of the research described [here](/observers)
   - Observer constructed by leveraging the symmetry of aircraft dynamics under the action of the Lie group SO(3)
2. **Passivity-based wind estimation**  
   - Leverage theory of feedback passivation to contruct a state observer  
   - Energy of the wind estimate error grows no faster than the energy of disturbances and uncertainties

## Why It Matters  
- **Synthetic air data systems**: Reconstruct airspeed, angle of attack, and sideslip without dedicated sensors, providing redundancy and resilience in sensor-limited operations.  
- **Path planning and control**: Incorporate real-time wind estimates to improve efficiency, safety, and weather tolerance --- essential for future urban and advanced air mobility missions.  
- **Atmospheric science**: Provide new tools to study the atmospheric boundary layer, which remains under-sampled due to operational constraints of traditional platforms.  

## Selected Publications  
- *[Nonlinear Wind Estimation Using a Symmetry-Preserving Reduced-Order Observer](/publications/#hopwoodNonlinearWindEstimation2025)* --- Introduces a nonlinear reduced-order observer for wind estimation with global exponential stability guarantees, demonstrated on multirotor and fixed-wing aircraft models.  
- *[A Noise-to-State Stable Symmetry-Preserving Reduced-Order Observer for Wind Estimation](/publications/#hopwoodNoisetostateStableSymmetrypreserving2025)* --- Extends symmetry-preserving wind observers to the stochastic setting, providing probabilistic guarantees under turbulence and model uncertainty.  
- *[Model-Based Wind Estimation Using H∞ Filtering with Flight-Test Results](/publications/#gahanModelbasedWindEstimation2025)* --- Presents an H∞ filtering approach to wind estimation that estimates a desired frequency band of the wind despite unmodeled turbulence.
- *[Unsteady Aerodynamics in Model-Based Wind Estimation from Fixed-Wing Aircraft Motion](/publications/#halefomUnsteadyAerodynamicsModelbased2024)* --- Investigates the role of unsteady aerodynamic models in improving wind estimation accuracy.  
- *[Uncertainty in Wind Estimates, Part 1: Analysis Using Generalized Polynomial Chaos](/publications/#gahanUncertaintyWindEstimates2024)* --- Uses generalized polynomial chaos to analyze how parametric uncertainty affects wind estimate precision.  
- *[Uncertainty in Wind Estimates, Part 2: H∞ Filtering Using Generalized Polynomial Chaos](/publications/#gahanUncertaintyWindEstimates2024a)* --- Implements our H∞ filtering approach on the polynomial-chaos-expanded system that governs how the statistics of the aircraft's state evolve over time.
- *[Passivity-Based Wind Estimation for Aircraft Maneuvering in Steady and Uniform Wind Fields](/publications/#hopwoodPassivitybasedWindEstimation2024)* --- Develops a nonlinear, passivity-based observer with global convergence guarantees, validated with fixed-wing flight test data.  
- *[Intelligent Wind Estimation for Chemical Source Localization](/publications/#cooperIntelligentWindEstimation2023)* --- Uses a large-domain, nonlinear aerodynamic model for multirotor aircraft in conjuction with an unscented Kalman filter to perform wind-aware chemical source localization with small UAVs.

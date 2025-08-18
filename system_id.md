---
layout: default
title: System Identification
permalink: /system_id/
---
# System Identification  
*Large-domain modeling, system identification, and flight test for UAVs*  

## Overview  
Accurate flight dynamic models are essential for model-based control, estimation, and autonomy. For UAVs, however, obtaining nonlinear models valid across a wide range of flight conditions is challenging. Traditional approaches often capture only small perturbations around a nominal condition, weakening the guarantees of any controller or estimator designed from them. Our research develops **nonlinear multirotor, fixed-wing, and vertical-takeoff-and-landing (VTOL) models** that balance accuracy and practicality, along with **system identification methods** that remain safe even for inherently unstable aircraft.

## Approach  
System identification for UAVs requires overcoming several challenges: nonlinear aerodynamics, instability, and the need for safe automated experiments. Our approach addresses these challenges through three main directions:  

1. **Nonlinear multirotor modeling**  
   - Models derived from blade-element and momentum theory, valid across diverse flight conditions  
   - Simplified forms enable tractable estimation and control design  

2. **Safe system identification for unstable aircraft**  
   - Framework leverages stability guarantees from a **robust LPV H<sub>2</sub>/H<sub>∞</sub> controller**  
   - Controller executes specially designed reference signals that **decorrelate model regressors**, ensuring accurate parameter estimation  
   - Enables rich input/output data collection without risking instability  

3. **Spin and stall dynamics modeling**  
   - Data-driven aerodynamic models for stall-spin regimes of fixed-wing UAVs  
   - Supports robust control design for extreme flight conditions  

## Why It Matters  
- **Safety assurance**: Stabilizes inherently unstable UAVs while performing aggressive excitation for system identification.  
- **Reliable identification**: Reference trajectories and robust control design mitigate regressor correlation, improving parameter estimation accuracy.  
- **Scalable methods**: Applicable to both small UAVs and larger, high-cost vehicles where model-free excitation is unsafe.  
- **Advanced autonomy**: Provides the modeling foundation needed for weather-tolerant and robust next-generation air mobility.  

## Selected Publications  
- *[Practical Nonlinear Flight Dynamic Modeling for Multirotor Aircraft](/publications/#hopwoodPracticalNonlinearFlight2025)* --- Develops compact nonlinear multirotor models valid across diverse conditions, balancing fidelity and identifiability.  
- *[Robust Linear Parameter-Varying Control for Safe and Effective Unstable Aircraft System Identification](/publications/#hopwoodRobustLinearParametervarying2024)* --- Introduces an LPV H₂/H∞ framework that stabilizes UAVs during excitation and executes decorrelating trajectories for accurate large-domain model identification.  
- *[Development and Evaluation of Multirotor Flight Dynamic Models for Estimation and Control](/publications/#hopwoodDevelopmentEvaluationMultirotor2024)* --- Presents nonlinear multirotor models derived from blade-element and momentum theory, validated through simulation and experiments.  
- *[Spin Aerodynamic Modeling for a Fixed-Wing Aircraft Using Flight Data](/publications/#greshamSpinAerodynamicModeling2024)* --- Identifies a nonlinear aerodynamic model for stall-spin regimes using flight test data, outperforming nominal models in extreme flight.  
- *[Remote Uncorrelated Pilot Input Excitation Assessment for Unmanned Aircraft Aerodynamic Modeling](/publications/#greshamRemoteUncorrelatedPilot2023)* --- Proposes techniques for ensuring pilot inputs yield uncorrelated data suitable for aerodynamic model identification.  
- *[Flight Test Approach for Modeling and Control Law Validation for Unmanned Aircraft](/publications/#greshamFlightTestApproach2022)* --- Demonstrates a progressive build-up approach to flight testing, combining system ID with nonlinear control validation.  
- *[Spin Aerodynamic Modeling for a Fixed-Wing Aircraft Using Flight Data](/publications/#greshamSpinAerodynamicModeling2022)* --- Early results on spin aerodynamic modeling with novel excitation signal design.  


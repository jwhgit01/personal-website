---
layout: default
title: Capabilities & Collaboration
permalink: /capabilities/
css: /assets/css/capabilities.css
---

# Capabilities & Collaboration

***Rigorous methods. Flight-tested evidence.***

We help government, industry, and research partners develop and validate UAV technologies for challenging real-world conditions, including agile maneuvering, flight in turbulence, and multi-domain collaborative autonomy.

The **Performance-Assured Control and Estimation (PACE) Lab** specializes in the gap between state-of-the-art theory and credible flight test evidence. We combine rigorous analysis with rapid UAV integration, software development and flight testing so that new methods are not only publishable, but practical and defensible.

[Discuss a project](#work-with-us) &ensp;•&ensp; [See demonstrated results](#demonstrated-results)

## Why PACE

- **Beyond nominal flight**
  
  We work in regions of flight and with novel vehicle configurations where conventional assumptions and approaches fail.

- **Designed to tackle uncertainty**
  
  Modeling error and external disturbances are not an afterthought. They an integral part of the design problem and resulting performance and safety guarantees.

- **Models that bridge the gap**
  
  We identify physics-based flight dynamic models that bridge the gap between traditional control-oriented models and high-fidelity computational models.

- **Rapid implementation and flight testing**
  
  We translate novel control and estimation methods into [PX4](https://px4.io/) and [ROS](https://www.ros.org/) through proven experimental workflows, spanning rigorous simulation and flight testing of small UAVs.

- **Leverage mathematical structure**
  
  Our control, estimation, and autonomy technologies leverage dynamical system structure (e.g., symmetry, invariance, passivity) to improve performance, robustness, and safety assurances.
{: .capabilities-intro }

Our distinctive capability is the connection among three activities that are often separated: **nonlinear aircraft modeling**, **control and estimation with performance guarantees**, and **experimental flight validation**.

## Problems we help solve

Partners come to us when they need to:
- characterize a new, unconventional, or poorly modeled aircraft;
- evaluate a controller, estimator, sensor, or autonomy algorithm;
- operate safely beyond nominal flight conditions;
- infer wind or aerodynamic states without relying on dedicated sensors;
- translate novel robotics concepts to the aerial domain; or
- design UAV ground test and/or flight test campaigns.

## An integrated capability from modeling to flight

1. ### Design, instrument, and integrate UAVs

   ![Instrumented multirotor research UAV on a laboratory workbench](/assets/img/racer.jpg)

   Design and configure multirotor, fixed-wing, and eVTOL platforms with new sensors, payloads, and flight control software.

   **Tools:** PX4, ROS 1 & 2, MATLAB, SIL/HIL, UAVCAN/DRONECAN

2. ### Identify aircraft flight dynamics

   ![Force and moment residuals from nonlinear multirotor modeling](/assets/img/hopwoodLargedomainNonlinearSystem2024.jpg)

   Identify uncertainty-quantified models from flight data for use in nonlinear control and estimation.

   **Techniques:** Equation Error, Output Error, Machine Learning, Multivariate Orthogonal Function Modeling, Stepwise Regression

3. ### Control and estimation design

   ![Parallel control architecture for robust stall spin control](/assets/img/hopwoodStallSpinFlight2022.jpg)

   Develop safety-assured control laws and state/disturbance estimators for uncertain and stochastic nonlinear systems.

   **Bodies of Theory:** Differential Geometry, Passivity-Based Control, Invariant EKF, Robust H<sub>∞</sub> Control & Filtering, Stochastic Stability

4. ### Flight test validation

   ![eSPAARO fixed-wing UAV go-around during flight testing](/assets/img/eSPAARO-go-around.jpg)

   Build evidence through simulation, SIL/HIL, controlled wind experiments,
   and outdoor flight tests, increasing risk in stages.

   **Facilities:** MSU [North Farm](https://www.mafes.msstate.edu/branches/mainstation.php?location=foil) and [South Farm](https://www.mafes.msstate.edu/branches/mainstation.php?location=leveck), Raspet [Wind Wall](https://www.msstate.edu/newsroom/article/2025/03/msu-state-art-wind-lab-marks-new-era-national-drone-testing) and [motion capture system](https://www.ae.msstate.edu/research/asrl/), Low-speed wind tunnel
{: .capabilities-pipeline }

## Attritable air data system

Our custom small UAS air data units provide open and adaptable alternatives to conventional commercial probes. The designs emphasize low cost, 3D-printable construction, replaceable components, and configurations tailored to high-risk UAV flight testing.

- [**GitHub Repository**](https://github.com/jwhgit01/Attritable-Air-Data)
- *Documentation site coming soon*

![Fixed-wing UAV equipped with a wing-mounted air-data probe](/assets/img/espaaro_adu.jpg){:width="40%" height="auto" .center}

![VTOL UAV equipped with a multidirectional air-data probe](/assets/img/mtd4_adu.jpg){:width="40%" height="auto" .center}

## Research aircraft

Our go-to aircraft are selected for fast modification, modularity, and risk mitigation.
- *Technical specifications coming soon*
- **eVTOL Aircraft In Development**

![Fox fixed-wing UAV](/assets/img/research-aircraft/fox-with-students.webp)
![RACER quadrotor UAV](/assets/img/research-aircraft/racer.jpg)
{: .side-by-side-gallery }

## Demonstrated results
{: #demonstrated-results }

### Wind estimation and synthetic air data

We developed model-based wind estimators and demonstrated their rigorous convergence guarantees using fixed-wing and multirotor flight test data.
- [Leverage symmetry to design a reduced-order observer](/assets/papers/hopwoodSymmetryPreservingReducedOrderWind2026.pdf)
- [Use stochastic calculus to prove robustness to turbulence](/assets/papers/hopwoodNoisetostateStableSymmetrypreserving2025.pdf)
- [Estimate bulk atmospheric flows using robust filtering](/assets/papers/gahanModelbasedWindEstimation2025.pdf)
- [Incorporate unsteady aerodynamics into model-based algorithms](/assets/papers/halefomUnsteadyAerodynamicsModelbased2024.pdf)
- [Use an energy-based perspective to handle maneuvering flight](/assets/papers/hopwoodPassivitybasedWindEstimation2024.pdf)
- [Improve computational aspects of UAV-based wind profiling](/assets/papers/medinaEvaluationDopplerWind2025.pdf)
- [Mitigate uncertainty and wind estimate sensitivity to modeling error](/assets/papers/gahanWindEstimateUncertainty2026.pdf)
- [Use wind estimates for bio-inspired source localization](/assets/papers/cooperIntelligentWindEstimation2023.pdf)

### Aircraft system identification

We derived identifiable, physics-informed models for model-based design and developed techniques to identify these models from flight data.
- [Derive an evaluate a physics-based model for nonlinear multirotor aerodynamics](/assets/papers/hopwoodPracticalNonlinearFlight2026.pdf)
- [Leverage robust control to safely obtain information-rich flight data for unstable aircraft](/assets/papers/hopwoodRobustLinearParametervarying2024.pdf)
- [Model and identify stall spin aerodynamics from flight data](/assets/papers/greshamSpinAerodynamicModeling2024.pdf)
- [Lower the barrier to nonlinear model identification](/assets/papers/greshamRemoteUncorrelatedPilot2023.pdf)
- [Identify a control-oriented model of fixed-wing unsteady aerodynamics](/assets/papers/halefomUnsteadyAerodynamicsModelbased2024.pdf)
- [Open-source small UAV flight testing and control law evaluation](/assets/papers/greshamFlightTestApproach2022.pdf)

### Stall-spin modeling and flight termination systems

We identified nonlinear spin dynamics from flight data, designed robust stall spin flight termination methods, and validated these approaches through small UAV flight testing.
- [Robustly guide the spinning descent along a desired direction](/assets/papers/hopwoodRobustStallSpin2023.pdf)
- [Model and identify stall spin aerodynamics from flight data](/assets/papers/greshamSpinAerodynamicModeling2024.pdf)

## Work with us
{: #work-with-us }

We work with academic, government, and industry partners through sponsored and joint research, proposal teams, independent technology evaluation, payload and platform integration, and focused wind-tunnel or flight-test campaigns.

> **Bring us the difficult part.**
>
> If you have an aircraft, sensor, autonomy technology, or operating condition that needs credible modeling and experimental evidence, send a short description of the system, the conditions in which it must operate, and what you need to demonstrate.
>
> [**Discuss a research or test problem**](mailto:jhopwood@ae.msstate.edu?subject=PACE%20Lab%20collaboration%20inquiry)
{: .capabilities-contact }

---
layout: default
title: Nonlinear Observers
permalink: /observers/
---

# Nonlinear State Estimation & Observer Design  
*Mathematical foundations for reliable autonomy in nonlinear systems*  

## Overview  
Reliable state estimation is at the core of every autonomous system. Whether it's an aircraft navigating turbulence, a self-driving car handling unexpected road conditions, or an underwater vehicle operating without GPS, these systems must accurately infer their state.  

In linear systems, observer design is well established, with powerful techniques that guarantee global convergence. But in nonlinear settings where approximations break down and uncertainty dominates, these guarantees largely disappear. Our research aims to close this gap by developing estimation methods that not only work in practice, but are provably accurate.  

## Approach  
General-purpose observer design for nonlinear systems remains an open challenge: no universal technique exists to ensure global convergence. Instead, provably effective methods can only be built for special classes of systems.  

Our focus is on **systems with symmetry** --- systems whose dynamics remain unchanged under certain transformations. For example, the equations governing a drone's flight look the same regardless of its absolute position in space. By exploiting a syetem's structure, we can turn an otherwise intractable nonlinear observer design problem into one that admits constructive, rigorous solutions. 

The outcome is a set of estimation strategies that are not just heuristic, but mathematically grounded, giving stronger safety and performance guarantees for autonomous systems.  

## Why It Matters  
- **Safety-critical autonomy:** Ensures aircraft, cars, and robots make trustworthy decisions in uncertain environments.  
- **Beyond linear models:** Expands estimation theory into the nonlinear realm where most real-world systems live.  
- **Bridging theory and practice:** Provides constructive tools that engineers can implement with confidence.  

## Selected Publications  
- *[A Symmetry-Preserving Reduced-Order Observer](/publications/#hopwoodSymmetrypreservingReducedorderObserver2025)* --- Contructs a reduced-observer nonlinear observer by leveraging system symmetry.
- *More coming soon! See [Google Scholar](https://scholar.google.com/citations?hl=en&user=-kIX4SIAAAAJ) for a complete list.*  

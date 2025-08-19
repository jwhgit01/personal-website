---
layout: default
title: Nonlinear Observers
permalink: /observers/
---

# Nonlinear State Estimation & Observer Design  
*Mathematical foundations for autonomy in safety-critical systems*  

## Overview  
Provably accurate state estimation is at the core of developing trust in autonomous systems. Whether it's an aircraft maneuvering in turbulence, a self-driving car adapting to unexpected road conditions, or an underwater vehicle operating without GPS, these systems must accurately infer their state from available sensor data.  

In linear systems, observer design is well established, with powerful techniques that guarantee global convergence. But in nonlinear settings where approximations break down and uncertainty dominates, these guarantees largely disappear. Our research aims to close this gap by developing estimation methods that not only enjoy strong theoretical guarantees, but work in practice.

## Approach  
Observer design for general nonlinear systems remains an open challenge with no universal techniques existing that ensure global convergence. Instead, provably effective methods can only be built for special classes of systems.  

Our focus is on **systems with symmetry** --- that is, systems whose dynamics remain unchanged under certain transformations. For example, the equations governing a drone's flight are the same regardless of its absolute position in space. By exploiting a system's structure, we can turn an otherwise intractable nonlinear observer design problem into one that admits constructive, rigorous solutions. The outcome is a set of estimation strategies that are not just heuristic, but mathematically grounded, giving stronger **safety and performance guarantees** for autonomous systems.  

## Why It Matters  
- **Safety-critical autonomy:** Ensures aircraft, cars, and robots make trustworthy decisions in uncertain environments.  
- **Beyond linear models:** Expands estimation theory into the nonlinear regime where most real-world systems operate.  
- **Bridging theory and practice:** Provides constructive tools that engineers can implement with confidence.  

## Selected Publications  
- *[A Symmetry-Preserving Reduced-Order Observer](/publications/#hopwoodSymmetrypreservingReducedorderObserver2025)* --- Contructs a reduced-observer nonlinear observer by leveraging system symmetry.
- *More coming soon! See [Google Scholar](https://scholar.google.com/citations?hl=en&user=-kIX4SIAAAAJ) for a complete list.*  

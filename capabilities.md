---
layout: page
title: Lab Capabilities
subtitle: Rapid UAV development, flight testing, and air-data innovation
permalink: /capabilities/
---

The **Performance-Assured Control and Estimation (PACE) Lab** develops,
integrates, and experimentally validates technologies for multirotor,
fixed-wing, and electric vertical takeoff and landing (eVTOL) aircraft. We
combine low-cost UAV platforms, advanced simulation, flight testing, system
identification, air-data sensing, and state estimation to move ideas from
theory to flight-validated results.

<div class="capabilities-callout">
  <strong>What we offer:</strong> an integrated path from modeling and
  simulation through hardware integration, controlled testing, and outdoor
  flight validation.
</div>

## Rapid UAV development and flight testing

We rapidly configure and instrument small UAVs to evaluate new research
concepts, sensors, algorithms, and control systems.

<figure class="capabilities-figure">
  <img src="/assets/img/racer.jpg"
       alt="Instrumented multirotor UAV on a laboratory workbench">
  <figcaption>
    A modular multirotor research platform configured for rapid sensor,
    flight-computer, and algorithm integration.
  </figcaption>
</figure>

**Capabilities include:**

- Multirotor, fixed-wing, and eVTOL research platforms
- Custom payload and sensor integration
- Flight-computer and autopilot integration
- Rapid aircraft modification and prototyping
- ROS- and PX4-based development
- Experimental flight-test planning and execution
- Software-in-the-loop (SIL) and hardware-in-the-loop (HIL) testing

## Full-envelope system identification

We identify flight-dynamic models from experimental data collected throughout
the aircraft operating envelope, including nonlinear and off-nominal regimes
that are poorly represented by small-perturbation models.

**Relevant operating conditions include:**

- Aggressive and unsteady maneuvers
- Stall, post-stall, and spin behavior
- Low-speed flight
- eVTOL transition
- Rotor- and propeller-influenced flow
- Other nonlinear flight conditions

The resulting models support simulation, control development, aircraft
characterization, envelope expansion, and safety analysis. Learn more about
our [system-identification research](/system_id/).

<div class="capabilities-placeholder" role="img"
     aria-label="Placeholder for a system-identification results image">
  <span>Image placeholder</span>
  <strong>System-identification results</strong>
  <small>
    Suggested image: measured and model-predicted flight response across a
    nonlinear maneuver.
  </small>
</div>

## Wind estimation and synthetic air data

We develop algorithms that estimate wind and aerodynamic states from existing
onboard measurements and aircraft models.

**Estimated quantities may include:**

- Wind velocity
- Airspeed
- Angle of attack
- Sideslip angle

Synthetic air data can reduce dependence on specialized sensors and provide
information in operating regimes where conventional probes are ineffective.
This is particularly valuable near hover and during eVTOL transition. Learn
more about our [wind-estimation research](/wind_estimation/).

<div class="capabilities-placeholder" role="img"
     aria-label="Placeholder for a wind-estimation validation image">
  <span>Image placeholder</span>
  <strong>Wind-estimation validation</strong>
  <small>
    Suggested image: estimated wind compared with reference measurements from
    simulation, wind-tunnel testing, or flight.
  </small>
</div>

## Low-cost, open-source air-data unit

Our custom small-UAV air-data unit provides an accessible alternative to
conventional commercial probes.

<div class="capabilities-gallery capabilities-gallery--two">
  <figure class="capabilities-figure">
    <img src="/assets/img/espaaro_adu.jpg"
         alt="Fixed-wing UAV equipped with a wing-mounted air-data probe">
    <figcaption>
      Air-data instrumentation integrated on a fixed-wing research aircraft.
    </figcaption>
  </figure>
  <figure class="capabilities-figure">
    <img src="/assets/img/mtd4_adu.jpg"
         alt="VTOL UAV equipped with a multi-directional air-data probe">
    <figcaption>
      A multi-directional probe configured for low-speed and transition-flight
      testing.
    </figcaption>
  </figure>
</div>

**Key features:**

- Approximately one-tenth the cost of comparable commercial systems
- Open-source design
- Predominantly 3D-printable construction
- Compact, adaptable form factor
- Validation through wind-tunnel testing

The system supports flight-test instrumentation, aircraft characterization,
sensor validation, and synthetic-air-data research.

## Controlled wind-field testing

Mississippi State University's Raspet Flight Research Laboratory combines a
**large programmable fan array** with a motion-capture system. The facility can
generate spatially and temporally varying wind fields, enabling repeatable
experiments in which both vehicle motion and the surrounding flow are known.

<figure class="capabilities-figure capabilities-figure--portrait">
  <img src="/assets/img/20250219_094819.jpg"
       alt="Programmable fan array at the Raspet Flight Research Laboratory">
  <figcaption>
    The programmable fan array supports repeatable testing in controlled,
    spatially varying wind fields.
  </figcaption>
</figure>

**Applications include:**

- Gust-response testing
- Disturbance-rejection research
- Wind-aware guidance and control
- Wind-estimation validation
- Flight-dynamic system identification
- Controlled indoor vehicle testing

## End-to-end research workflow

<ol class="capabilities-workflow" aria-label="PACE Lab research workflow">
  <li>Theory</li>
  <li>Modeling</li>
  <li>Simulation</li>
  <li>SIL/HIL testing</li>
  <li>Integration</li>
  <li>Controlled testing</li>
  <li>Flight testing</li>
  <li>Validation</li>
</ol>

This integrated workflow provides a rapid path from a new research concept to
experimentally validated flight results. It also lets us introduce risk in
stages, resolve integration issues early, and collect the evidence needed to
evaluate performance.

## Collaboration areas

We welcome collaborations with academic, government, and industry partners
whose work would benefit from small-aircraft development and experimental
validation. Potential collaborations include:

- Sponsored and jointly developed research projects
- Independent evaluation of sensors, algorithms, and control systems
- UAV platform and payload integration
- Focused wind-tunnel, fan-array, or outdoor flight-test campaigns
- Flight-data collection, model development, and system identification
- Wind-estimation and synthetic-air-data demonstrations

If you have a research question, technology, or test objective that aligns with
these capabilities, contact
[Dr. Jeremy Hopwood](mailto:jhopwood@ae.msstate.edu) to discuss scope, platform
needs, facilities, and a path to validation.

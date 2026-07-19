# Model Scope and Interpretation

This document describes what the application represents and, equally
importantly, what it does not represent.

## Basic relative-value model

The Basic view uses a simplified mass-balance-style model with a completely
mixed assumption. The scalar value, source rate, reduction rate, and auxiliary
unit conversion are educational abstractions. They are not calibrated to a
specific substance, room, river, process, exposure limit, or measurement
instrument.

## Three-dimensional scalar field

The 3D Field view numerically advects an internal dye field for visualization.
Its grid, boundary behavior, turbulence-like motion, numerical diffusion,
rendering, and quality adaptation are designed for interactive learning rather
than validated CFD analysis.

The simulated sensor value is read from the internal GPU field and is not a physical sensor measurement.

## Riverbed morphology

The riverbed model updates an internal bed texture from a simplified simulated
near-bed shear metric and mobile-sediment quantity. Erosion, deposition, and
avalanche terms are illustrative numerical rules.

The following are not represented with site-specific physical fidelity:

- grain-size distributions or cohesive behavior;
- bed material properties;
- turbulence closure and near-wall physics;
- free-surface flow, water depth, hydraulic radius, or real discharge;
- sediment supply, armoring, vegetation, structures, or bank failure;
- calibrated erosion thresholds, transport capacity, or deposition velocity;
- survey datum, spatial scale, time scale, or uncertainty validation.

The UI field `terrainReliefCm` is a visualization-derived riverbed-relief conversion in `cm` from the internal bed amplitude. It must not be interpreted as measured or predicted
real-world elevation change.

## Uncertainty view

The uncertainty view combines a log-normal prior with a likelihood based on
synthetic demonstration data. It teaches the structure of updating a
distribution; it does not estimate a real-world parameter or provide validated
confidence or credible intervals for a real system.

## Fallback and device differences

When required WebGL2 capabilities are unavailable, the application uses a
visual fallback. The fallback does not reproduce every GPU-fluid or morphology
feature. Results and appearance can also differ with browser, GPU, driver,
device temperature, screen size, and quality adaptation.

## Appropriate use

Use the application to explore qualitative relationships, interface behavior,
and model structure. Any real-world decision requires independently selected,
validated, and calibrated methods together with suitable measurements and
qualified professional review.

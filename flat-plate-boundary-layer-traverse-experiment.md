# Flat-plate boundary-layer traverse experiment

↑ **Parent:** [Blasius boundary layer](blasius-boundary-layer.md)

The Louisiana Tech [LAB 8 - Velocity Profile above a Flat Plate](me-354-thermofluids-laboratory/lab-8-velocity-profile-above-a-flat-plate.md) describes a 14-inch plate in a [wind tunnel](wind-tunnel.md). A [Pitot-static tube](pitot-static-tube.md) of 0.10-inch outside diameter traverses normally about 12 inches downstream; its screw scale has 0.001-inch increments. A water-column [manometer](manometer.md) reads the difference between [stagnation pressure](stagnation-pressure.md) and [static pressure](static-pressure.md). The procedure establishes a wall position, zeros the tunnel indicator, sets fan speed, and records at least ten positions inside the [boundary layer](boundary-layer.md), together with room [temperature](temperature.md) and barometric [pressure](pressure.md). The instrument list includes a flow-stream [thermometer](thermometer.md) implemented with a temperature-sensitive resistor. The manual requests comparison of outer [velocity](velocity.md) with the tunnel indicator and of the recovered [velocity profile](velocity-profile.md) with laminar or turbulent predictions; it provides no observed dataset. These are apparatus specifications and instructions, not a reported confirmation of [laminar flow](laminar-flow.md).

<a id="image-pressure-based-sampling-model-for-a-flat-plate-velocity-traverse"></a>
![](flat-plate-velocity-traverse-apparatus.png)

**[Figure 2](#image-pressure-based-sampling-model-for-a-flat-plate-velocity-traverse). Pressure-based sampling model for a flat-plate velocity traverse**. An original [wind tunnel](wind-tunnel.md) apparatus schematic and synthetic [Blasius boundary layer](blasius-boundary-layer.md) readout. Hollow points are idealized averages of [dynamic pressure](dynamic-pressure.md) over a hypothetical $0.50\,\mathrm{mm}$ normal sampling footprint, not laboratory observations or the quoted probe bore. No sample centre reaches the wall. The schematic exaggerates normal distances and tubing spacing.

Under [incompressible flow](incompressible-flow.md) conditions, an ideal aligned [Pitot tube](pitot-tube.md) gives $q(y)=p_0(y)-p(y)=\rho u(y)^2/2$. Convert the [manometer](manometer.md) head $h$ to $q=(\rho_{\mathrm{water}}-\rho)gh$, then infer $u=\sqrt{2q/\rho}$. Here $g$ is [gravitational acceleration](gravitational-acceleration.md); [mass density](density.md) $\rho$ can be estimated from [temperature](temperature.md) and absolute [pressure](pressure.md) using the [ideal gas law](ideal-gas-law.md). A normalized [velocity profile](velocity-profile.md) rises from the unresolved near-wall region to a plateau, whose value defines $U$; downstream profiles should broaden and collapse when plotted against $\eta$ if the [Blasius boundary layer](blasius-boundary-layer.md) assumptions hold. Integrating a recovered [velocity profile](velocity-profile.md) gives [displacement thickness](displacement-thickness.md) and [momentum thickness](momentum-thickness.md).

Additional controls for interpreting this experiment follow from the measurement model: check [differential-pressure calibration](differential-pressure-calibration.md) with equal port [pressures](pressure.md) and known liquid heads; leak-check tubing; align the [Pitot tube](pitot-tube.md) with the incoming [velocity](velocity.md); convert wall contact to the inlet-centre coordinate rather than treating outside contact as $y=0$; repeat traverses and outer [velocity](velocity.md) readings to detect drift. Keep the plate smooth and aligned, and check outer [static pressure](static-pressure.md) at multiple downstream stations before assuming zero [pressure gradient](pressure-gradient.md). Repeating at another station or outer [velocity](velocity.md) tests the predicted [boundary-layer scaling](boundary-layer-scaling.md) more directly than fitting one curve. These controls are proposed checks, not actions documented as completed in the manual.

Finite probe size, wall interference, flow fluctuations, and weak near-wall [dynamic pressure](dynamic-pressure.md) limit inference. Even the manual's probe-based [Reynolds number](reynolds-number.md) criterion, $\mathrm{Re}_d=ud/\nu>1000$ for its ideal [Bernoulli equation](bernoulli-equation.md) conversion, must be checked with local $u$, not just $U$. In the illustrative model at $x=0.3048\,\mathrm m$, $\delta_{99}\simeq3.32\,\mathrm{mm}$; the quoted outside diameter is $2.54\,\mathrm{mm}$, a substantial fraction of that thickness. A real inlet's sensing footprint and correction cannot be deduced from outside diameter alone. For an ideal footprint that averages [dynamic pressure](dynamic-pressure.md), the inferred [velocity](velocity.md) is $\sqrt{\langle u^2\rangle}$ rather than $\langle u\rangle$. Differentiating such sparse readings to obtain [wall shear stress](wall-shear-stress.md) magnifies [measurement error](measurement-error.md); the [momentum thickness](momentum-thickness.md) route is less sensitive to this differentiation but still needs the unresolved near-wall contribution. The [no-slip boundary condition](no-slip-boundary-condition.md) is a model constraint here, not a direct reading from a probe centred on the wall.

## ↑ Ancestors (6)

1. [Blasius boundary layer](blasius-boundary-layer.md)
2. [Boundary layer](boundary-layer.md)
3. [Continuum mechanics](continuum-mechanics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Blasius boundary layer](blasius-boundary-layer.md)

# Lift (force)

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lift_(force))

[Lift](lift-force.md) is the component of the [fluid](fluid-mechanics.md#fluid) [force](force.md) perpendicular to the far-field flow relative to the body. It need not point vertically: a tilted flow changes the lift direction, and a banked wing can produce a sideways component. In a planar problem choose a unit [vector](vector-space.md#vector) $\mathbf e_D$ along the incoming relative [velocity](classical-mechanics.md#velocity) $\mathbf U_\infty$ and a perpendicular unit [vector](vector-space.md#vector) $\mathbf e_L$ pointing towards the chosen positive-lift side. Then

$$
U_\infty=|\mathbf U_\infty|,\qquad
D=\mathbf F\cdot\mathbf e_D,\qquad
L=\mathbf F\cdot\mathbf e_L,\qquad
\mathbf F=D\mathbf e_D+L\mathbf e_L.
$$

Here $D$ is [drag](fluid-mechanics.md#drag-physics) and $L$ is signed [lift](lift-force.md); $L<0$ means a [force](force.md) towards the opposite side. In three dimensions the plane perpendicular to $\mathbf U_\infty$ also admits a separate side-force direction, so a lift axis must be specified. [Lift](lift-force.md) is also distinct from [buoyancy](fluid-mechanics.md#buoyancy), which can exist without a relative flow. [NASA Glenn, Aerodynamic Forces: components relative to the flow](https://www1.grc.nasa.gov/beginners-guide-to-aeronautics/aerodynamic-forces/)

The [force](force.md) comes from adding local surface [tractions](continuum-mechanics.md#traction), rather than assigning a single [pressure](pressure.md) to each side. Let $\Sigma$ be the wetted body surface and $\mathbf n$ its unit [normal vector](differential-geometry.md#normal-vector) pointing out of the body into the [fluid](fluid-mechanics.md#fluid). The [pressure](pressure.md) contribution pushes inwards; the [viscous stress tensor](dynamic-viscosity.md#viscous-stress-tensor) also contributes, including tangential [shear stress](viscous-fluid-flow.md#shear-stress):

$$
\mathbf F=\int_\Sigma\left[-(p-p_\infty)\mathbf n+\boldsymbol\sigma_{\mathrm{visc}}\mathbf n\right]dA,
\qquad
L=\int_\Sigma\left[-(p-p_\infty)\mathbf n+\boldsymbol\sigma_{\mathrm{visc}}\mathbf n\right]\cdot\mathbf e_L\,dA.
$$

Using a constant reference [pressure](pressure.md) $p_\infty$ is legitimate on a closed surface because $\int_\Sigma\mathbf n\,dA=0$. This [surface integral](multivariable-calculus.md#surface-integral) makes the direction explicit: a surface-normal [force](force.md) is generally neither pure [lift](lift-force.md) nor pure [drag](fluid-mechanics.md#drag-physics). [Pressure](pressure.md) and skin [shear stress](viscous-fluid-flow.md#shear-stress) both enter the resultant, although the [pressure](pressure.md) term usually dominates [lift](lift-force.md) on an [airfoil](fluid-mechanics.md#airfoil). [NASA Glenn, Aerodynamic Forces: pressure and shear contributions](https://www1.grc.nasa.gov/beginners-guide-to-aeronautics/aerodynamic-forces/)

<a id="image-local-pressure-forces-and-lift-relative-to-the-far-field-flow"></a>
![](lift-airfoils-pressure-geometry.png)

**[Figure 1](#image-local-pressure-forces-and-lift-relative-to-the-far-field-flow). Local pressure forces and lift relative to the far-field flow**. Original toy geometry: a thin diamond-shaped section at $10\,{}^\circ$ [angle of attack](fluid-mechanics.md#angle-of-attack), with prescribed [pressure coefficients](#pressure-coefficient) $C_{p,u}=-0.8(1-x/c)$ above and $C_{p,l}=0.4(1-x/c)$ below. Arrows show gauge-pressure contributions: negative gauge pressure gives an outward contribution after the uniform ambient pressure has cancelled over the closed surface. The right panel resolves the integrated pressure force into flow axes. These prescribed pressures are neither measured data nor a solved flow; the corners and thickness are illustrative.

The [lift coefficient](#lift-coefficient) isolates a useful scale. For a finite wing of reference area $S$ (normally its projected planform area), and for a two-dimensional [airfoil](fluid-mechanics.md#airfoil) section of chord length $c$, respectively,

$$
q_\infty=\frac12\rho_\infty U_\infty^2,\qquad
C_L=\frac{L}{q_\infty S},\qquad
c_l=\frac{L'}{q_\infty c}.
$$

Here $q_\infty$ is [dynamic pressure](#dynamic-pressure), $\rho_\infty$ is far-field [mass density](fluid-mechanics.md#density), and $L'$ is [lift](lift-force.md) per unit span, with units $\mathrm{N\,m^{-1}}$. The signs of $C_L$ and $c_l$ follow the chosen lift axis. For stipulated values $\rho_\infty=1.20\,\mathrm{kg\,m^{-3}}$, $U_\infty=20\,\mathrm{m\,s^{-1}}$, $S=0.50\,\mathrm{m^2}$ and $C_L=0.60$, $q_\infty=240\,\mathrm{Pa}$ and $L=72\,\mathrm N$. Doubling $U_\infty$ gives four times the [lift](lift-force.md) only if $C_L$ stays fixed: changes in [Reynolds number](dynamic-viscosity.md#reynolds-number), [Mach number](compressible-flow.md#mach-number), surface condition or [angle of attack](fluid-mechanics.md#angle-of-attack) can change it. [NASA Glenn, Lift Coefficient: normalization and similarity limits](https://www1.grc.nasa.gov/beginners-guide-to-aeronautics/lift-coefficient/)

A motivating experiment is to compare two independently observed quantities: the [lift](lift-force.md) registered by a force balance, and the [lift](lift-force.md) inferred from surface [pressures](pressure.md). A low-speed wind tunnel holds the model fixed while air passes it at adjustable speed; a calibrated balance measures [forces](force.md), while small flush holes on both surfaces connect by tubing to differential-pressure sensors referenced to $p_\infty$. Iowa State's GA(W)-1 teaching model has $43$ taps around a $101\,\mathrm{mm}$ chord; its instructions give their coordinates and close the contour by repeating the first tap. A classroom comparison can combine this pressure-panel method with a balance on the same model; this is an experiment design, not a claim that those instructions report a combined measurement. [Hui Hu, Iowa State, AerE344 Lab 05, p. 2: GA(W)-1 taps and pressure panels](https://www.aere.iastate.edu/~huhui/teaching/2026-08F/AerE344/lab-instruction/AerE344L-Lab-05-Pressure-Airfoil-instruction.pdf) [NASA Glenn, Drag Measurement: force balances and calibration](https://www1.grc.nasa.gov/beginners-guide-to-aeronautics/drag-measurement/)

<a id="image-compare-a-force-balance-with-integrated-airfoil-pressure-measurements"></a>
![](lift-airfoils-wind-tunnel.png)

**[Figure 2](#image-compare-a-force-balance-with-integrated-airfoil-pressure-measurements). Compare a force balance with integrated airfoil pressure measurements**. Original schematic of a proposed low-speed experiment, not a drawing of a particular facility. The model has a rotatable mount, surface taps and two independent measurement routes. Only a few taps are drawn. A far-field total/static pressure probe supplies the speed scale; balance calibration uses known loads, and pressure calibration uses known pressure differences. No measured curves or results are shown.

Before turning on the wind, apply known positive and negative loads to the balance through its resolving centre; use $mg$ for the known load from a mass. Record all balance channels during loading and unloading, including response to [drag](fluid-mechanics.md#drag-physics) and [torque](momentum.md#torque) loads, to detect cross coupling, hysteresis and zero drift. Record a wind-off tare at each model orientation so its [weight](semisimple-lie-algebra.md#weight-representation-theory) does not become an aerodynamic [lift](lift-force.md) reading. Map tunnel flow direction and uniformity, rather than using the fan setting as a speed measurement. Covert's MIT guide describes these calibration, tare and flow-survey requirements. [Eugene E. Covert, A Student's Introduction to the Wright Brothers Wind Tunnel at MIT, pp. 3–8](https://ocw.mit.edu/courses/16-621-experimental-projects-i-spring-2003/f38ecde8773fd36c0d8f9069e6aa1df5_student_wt_guide.pdf)

For each pressure channel, apply zero and several known [pressure](pressure.md) differences spanning the expected range; determine the voltage-to-pressure relation and recheck it after a run. Inspect tubing for leaks and blocked taps, and wait for readings to settle before averaging: tubing can delay a pressure signal. This calibration principle is used in NASA's electronically scanned pressure systems, where several applied calibration pressures determine each sensor's response and repeated calibration tracks drift. A simple pressure standard can instead use a liquid-column height difference and the [hydrostatic pressure](fluid-mechanics.md#hydrostatic-pressure) law. [Patsy S. Fulton, NASA-TM-101531, p. 8: pressure-module calibration](https://ntrs.nasa.gov/api/citations/19890009044/downloads/19890009044.pdf)

Measure far-field static and total [pressure](pressure.md) outside the model's [fluid wake](fluid-mechanics.md#wake-physics); in low-speed [incompressible flow](fluid-mechanics.md#incompressible-flow) their difference gives $q_\infty$ by the [Bernoulli equation](euler-equations-for-an-inviscid-fluid.md#bernoulli-equation), so $U_\infty=\sqrt{2q_\infty/\rho_\infty}$. Record [temperature](temperature.md) and ambient [pressure](pressure.md) to determine [mass density](fluid-mechanics.md#density) using the [ideal gas law](ideal-gas.md#ideal-gas-law). At fixed $q_\infty$, step the [angle of attack](fluid-mechanics.md#angle-of-attack), repeat selected settings, and sweep back down to check reproducibility. Record balance [lift](lift-force.md), each tap's mean [pressure](pressure.md), and fluctuation sizes. NASA describes pressure probes connected to differential transducers and emphasizes recording their reference [pressure](pressure.md). [NASA Glenn, Total Pressure Measurement: probes, tubing and pressure references](https://www.grc.nasa.gov/www/k-12/airplane/tunptm.html)

Convert each tap to a [pressure coefficient](#pressure-coefficient) $C_{p,i}=(p_i-p_\infty)/q_\infty$. For consecutive taps bounding a panel of length $\Delta s_i$ with outward [normal vector](differential-geometry.md#normal-vector) $\mathbf n_i$, a [trapezoidal rule](runge-kutta-method.md#trapezoidal-rule) estimate of the pressure [force](force.md) per unit span is

$$
\mathbf F'_p\simeq-q_\infty\sum_i\frac{C_{p,i}+C_{p,i+1}}2\mathbf n_i\Delta s_i,\qquad
L'_p=\mathbf F'_p\cdot\mathbf e_L.
$$

Compare this with balance [lift](lift-force.md) divided by span only when the spanwise flow is approximately uniform. Agreement tests the pressure-resultant picture; disagreement calls for checking unresolved leading-edge pressure variations, skin [shear stress](viscous-fluid-flow.md#shear-stress), support loads and three-dimensional end effects before rejecting it. A force balance senses the total load, while taps alone reconstruct the pressure part. Tunnel walls and model blockage alter the effective flow and require corrections; end plates or a model extending between walls approximate two-dimensional flow but do not guarantee it. Record the [Reynolds number](dynamic-viscosity.md#reynolds-number) and [Mach number](compressible-flow.md#mach-number) with the result, and do not interpret tunnel [lift coefficients](#lift-coefficient) as universal wing data. [Covert, pp. 8–9: flow characterization and wall effects](https://ocw.mit.edu/courses/16-621-experimental-projects-i-spring-2003/f38ecde8773fd36c0d8f9069e6aa1df5_student_wt_guide.pdf) [NASA Glenn, Lift Coefficient: Reynolds and Mach number dependence](https://www1.grc.nasa.gov/beginners-guide-to-aeronautics/lift-coefficient/)

**Table of contents**

- [Lift coefficient](#lift-coefficient)
  - [Dynamic pressure](#dynamic-pressure)
- [Pressure coefficient](#pressure-coefficient)
  - [Pressure tapping](#pressure-tapping)

## Lift coefficient

↑ **Parent:** [Lift (force)](lift-force.md)

The signed [lift](lift-force.md) divided by [dynamic pressure](#dynamic-pressure) times a stated reference area. For a two-dimensional [airfoil](fluid-mechanics.md#airfoil), use $c_l=L'/(q_\infty c)$ instead. Reference area and experimental flow conditions are part of the definition of a reported coefficient; see [lift](lift-force.md) for a worked scale and a pressure/balance experiment.

### Dynamic pressure

↑ **Parent:** [Lift coefficient](#lift-coefficient)

[Dynamic pressure](#dynamic-pressure) is the bulk [kinetic energy](energy.md#kinetic-energy) per unit [volume](geometry-and-topology.md#volume) associated with [fluid](fluid-mechanics.md#fluid) motion at [speed](classical-mechanics.md#speed) $U$ in a specified [reference frame](mathematical-physics.md#reference-frame):

$$
q=\frac12\rho U^2,\qquad
\frac{\tfrac12mU^2}{V}=\frac12\rho U^2,\qquad
\mathrm{J\,m^{-3}}=\mathrm{Pa}.
$$

Here $\rho=m/V$ is [mass density](fluid-mechanics.md#density). The word "pressure" identifies its units and its use as a [pressure](pressure.md) scale; $q$ is not an extra isotropic [stress](continuum-mechanics.md#stress) to add to the local [static pressure](fluid-mechanics.md#static-pressure) in every surface [traction](continuum-mechanics.md#traction). A stationary [fluid](fluid-mechanics.md#fluid) can have large [static pressure](fluid-mechanics.md#static-pressure) with $q=0$. Conversely, knowing $U$ and $\rho$ fixes $q$ without fixing [static pressure](fluid-mechanics.md#static-pressure). The definition remains useful in [viscous fluid flow](viscous-fluid-flow.md) and [compressible flow](compressible-flow.md), even when the simplest [Bernoulli equation](euler-equations-for-an-inviscid-fluid.md#bernoulli-equation) is inapplicable. [Dynamic Pressure by NASA Glenn Research Center](physics-bibliography.md#dynamic-pressure-by-nasa-glenn-research-center)

For stipulated [mass density](fluid-mechanics.md#density) $\rho_\infty=1.20\,\mathrm{kg\,m^{-3}}$ and reference [speed](classical-mechanics.md#speed) $U_\infty=20\,\mathrm{m\,s^{-1}}$, $q_\infty=240\,\mathrm{Pa}$. At $40\,\mathrm{m\,s^{-1}}$ with the same [mass density](fluid-mechanics.md#density), $q_\infty=960\,\mathrm{Pa}$. This quadratic scaling makes [dynamic pressure](#dynamic-pressure) a useful normalization for the [lift coefficient](#lift-coefficient), [drag coefficient](fluid-mechanics.md#drag-coefficient) and [pressure coefficient](#pressure-coefficient); it predicts four times a particular [force](force.md) only if its corresponding coefficient remains unchanged.

<a id="image-a-pitot-static-tube-compares-stagnation-pressure-with-static-pressure"></a>
![](pitot-static-pressure-difference.png)

**[Figure 3](#image-a-pitot-static-tube-compares-stagnation-pressure-with-static-pressure). A Pitot-static tube compares stagnation pressure with static pressure**. Original schematic with separate [pressure](pressure.md) passages and a differential readout. The right panel uses stipulated values, not measurements: ideal stopping in [incompressible flow](fluid-mechanics.md#incompressible-flow) at unchanged height raises [static pressure](fluid-mechanics.md#static-pressure) by 240 Pa as the [kinetic energy](energy.md#kinetic-energy) per unit [volume](geometry-and-topology.md#volume) falls by 240 Pa. The diagram is not a probe design or a claim that real [static pressure](fluid-mechanics.md#static-pressure) ports are error free.

The connection with [stagnation pressure](fluid-mechanics.md#stagnation-pressure) requires hypotheses. For [steady flow](fluid-mechanics.md#steady-flow), constant [mass density](fluid-mechanics.md#density), [inviscid flow](fluid-mechanics.md#inviscid-flow), and [gravity](physics.md#gravity) as the only [body force](fluid-mechanics.md#body-force), the [Bernoulli equation](euler-equations-for-an-inviscid-fluid.md#bernoulli-equation) gives, along one [streamline](fluid-mechanics.md#streamline),

$$
p+\frac12\rho U^2+\rho gz=B.
$$

Here $p$ is [static pressure](fluid-mechanics.md#static-pressure), $g$ is [gravitational acceleration](newton-s-law-of-universal-gravitation.md#gravitational-acceleration), and $z$ is height. Bring that flow to rest without losses at the same height and the limiting [static pressure](fluid-mechanics.md#static-pressure) is the [stagnation pressure](fluid-mechanics.md#stagnation-pressure) $p_0$:

$$
p_0=p+q,\qquad p_0-p=\frac12\rho U^2.
$$

There must be no intervening pump supplying [work](energy.md#work) or other energy input. Constancy along one [streamline](fluid-mechanics.md#streamline) does not assert equal $B$ on all [streamlines](fluid-mechanics.md#streamline); [irrotational flow](vorticity.md#irrotational-flow) in a connected region supplies that additional conclusion. Changing height requires retaining $\rho gz$. In [compressible flow](compressible-flow.md) the stopping [pressure](pressure.md) difference generally differs from $\rho U^2/2$, and [viscous dissipation](stokes-flow.md#viscous-dissipation) can reduce recovered [stagnation pressure](fluid-mechanics.md#stagnation-pressure). [Bernoulli’s Equation by NASA Glenn Research Center](physics-bibliography.md#bernoulli’s-equation-by-nasa-glenn-research-center)

A [Pitot-static tube](fluid-mechanics.md#pitot-static-tube) turns this relation into a measurement: its upstream-facing opening senses [stagnation pressure](fluid-mechanics.md#stagnation-pressure), while separate side openings sample [static pressure](fluid-mechanics.md#static-pressure). Connect these to the positive and negative ports of a differential [pressure transducer](fluid-mechanics.md#pressure-transducer) or [manometer](fluid-mechanics.md#manometer). Under the hypotheses above, the measured difference $\Delta p$ gives

$$
U=\sqrt{\frac{2\Delta p}{\rho}}.
$$

Thus the stipulated $240\,\mathrm{Pa}$ and $1.20\,\mathrm{kg\,m^{-3}}$ imply $20\,\mathrm{m\,s^{-1}}$, not an independently measured [speed](classical-mechanics.md#speed). Align the probe with the incoming flow and keep its passages clear: blockage and pinched tubing invalidate the comparison. At very low [speed](classical-mechanics.md#speed), the difference can be smaller than instrument error; at high [Mach number](compressible-flow.md#mach-number), [compressibility](thermodynamics.md#compressibility) and possibly a [shock wave](transport-equation.md#shock-wave) require a different reduction. [Pitot – Static Tube – Speedometer by NASA Glenn Research Center](physics-bibliography.md#pitot-static-tube-speedometer-by-nasa-glenn-research-center)

A useful control is [differential-pressure calibration](fluid-mechanics.md#differential-pressure-calibration). For a digital [manometer](fluid-mechanics.md#manometer), zeroing establishes the reading at equal port [pressures](pressure.md); it does not establish the gain away from zero. The manufacturer's [Series 475 Handheld Digital Manometer: Specifications - Installation and Operating Instructions by Dwyer Instruments, Inc.](physics-bibliography.md#series-475-handheld-digital-manometer-specifications-installation-and-operating-instructions-by-dwyer-instruments-inc) directs the user to vent both ports to the atmosphere before zeroing. Its stated accuracy is a fraction of full scale, not of the reading, and depends on instrument [temperature](temperature.md). Select a suitable range and record the instrument variant and units; the manual covers several ranges.[p. 1: Specifications, Model Chart and ZERO instructions](physics-bibliography.md#series-475-handheld-digital-manometer-specifications-installation-and-operating-instructions-by-dwyer-instruments-inc)

An independent physical check can use a liquid-column [manometer](fluid-mechanics.md#manometer): apply a stable [pressure](pressure.md) difference to both instruments and compare the digital reading with the [hydrostatic pressure](fluid-mechanics.md#hydrostatic-pressure) inferred from the vertical level difference. For equal-height connections carrying a gas of [mass density](fluid-mechanics.md#density) $\rho_g$ above a manometric liquid of [mass density](fluid-mechanics.md#density) $\rho_m$,

$$
|\Delta p|=(\rho_m-\rho_g)g|h|.
$$

This follows by balancing [hydrostatic pressure](fluid-mechanics.md#hydrostatic-pressure) down and up the two connected columns. Use vertical height, even if a tube is inclined. Known [mass densities](fluid-mechanics.md#density), measured height and [gravitational acceleration](newton-s-law-of-universal-gravitation.md#gravitational-acceleration) set the comparison scale. Check several differences across the working range and reverse the port connections to check the sign. This is a proposed independent check, not a claim that the cited teaching experiment performed a full instrument calibration. Recheck zero after reconnecting the sealed tubing; a zero adjustment alone cannot detect a blocked passage or an incorrect scale.

## Pressure coefficient

↑ **Parent:** [Lift (force)](lift-force.md)

The [pressure coefficient](#pressure-coefficient) compares a local [static pressure](fluid-mechanics.md#static-pressure) with a specified reference [static pressure](fluid-mechanics.md#static-pressure), using a fixed reference [dynamic pressure](#dynamic-pressure):

$$
C_p(\mathbf x)=\frac{p(\mathbf x)-p_\infty}{q_\infty},\qquad
q_\infty=\frac12\rho_\infty U_\infty^2>0.
$$

The reference [mass density](fluid-mechanics.md#density), [speed](classical-mechanics.md#speed), [pressure](pressure.md) and location must accompany a reported [pressure coefficient](#pressure-coefficient). Keep the same $q_\infty$ throughout a surface distribution; replacing it by local $\rho U^2/2$ gives a different quantity and fails at a [stagnation point](fluid-mechanics.md#stagnation-point). The definition itself requires neither [Bernoulli's principle](euler-equations-for-an-inviscid-fluid.md#bernoulli-s-principle) nor [inviscid flow](fluid-mechanics.md#inviscid-flow), so measured [pressure coefficients](#pressure-coefficient) remain useful when those idealizations fail.

Positive $C_p$ means $p>p_\infty$; zero means equality; negative $C_p$ means $p<p_\infty$. This sign does not specify the sign of [absolute pressure](fluid-mechanics.md#absolute-pressure). For stipulated $p_\infty=101325\,\mathrm{Pa}$ absolute and $q_\infty=240\,\mathrm{Pa}$, $C_p=-3$ gives $p=100605\,\mathrm{Pa}$ absolute: a $720\,\mathrm{Pa}$ deficit, not a negative [absolute pressure](fluid-mechanics.md#absolute-pressure). If $p_\infty$ equals [atmospheric pressure](pressure.md#atmospheric-pressure), the numerator is [gauge pressure](fluid-mechanics.md#gauge-pressure); a [wind tunnel](fluid-mechanics.md#wind-tunnel)'s reference [static pressure](fluid-mechanics.md#static-pressure) need not equal room [atmospheric pressure](pressure.md#atmospheric-pressure). These are reference choices, not different physical [pressures](pressure.md).

Under the same-height, constant-[mass density](fluid-mechanics.md#density) $\rho=\rho_\infty$, [steady flow](fluid-mechanics.md#steady-flow) and [inviscid flow](fluid-mechanics.md#inviscid-flow) hypotheses of the [Bernoulli equation](euler-equations-for-an-inviscid-fluid.md#bernoulli-equation), and with the same [Bernoulli invariant](euler-equations-for-an-inviscid-fluid.md#bernoulli-invariant) as the reference flow,

$$
p+\frac12\rho U^2=p_\infty+\frac12\rho U_\infty^2,
\qquad C_p=1-\left(\frac{U}{U_\infty}\right)^2.
$$

The first equation immediately gives the second after subtracting $p_\infty$ and dividing by $q_\infty$. Hence a lossless [stagnation point](fluid-mechanics.md#stagnation-point) has $C_p=1$, $U=U_\infty$ gives $C_p=0$, and $U=2U_\infty$ gives $C_p=-3$. For a real stationary wall satisfying the [no-slip boundary condition](viscous-fluid-flow.md#no-slip-boundary-condition), the [velocity](classical-mechanics.md#velocity) is zero right at the wall; inserting that wall [velocity](classical-mechanics.md#velocity) in an [inviscid flow](fluid-mechanics.md#inviscid-flow) formula would wrongly predict $C_p=1$ everywhere. A thin [boundary layer](continuum-mechanics.md#boundary-layer) approximation instead relates the wall [pressure](pressure.md) to the outer-flow [pressure](pressure.md) and uses the outer [velocity](classical-mechanics.md#velocity) where the [Bernoulli equation](euler-equations-for-an-inviscid-fluid.md#bernoulli-equation) applies.

<a id="image-ideal-cylinder-pressure-coefficients-pressure-tapping-and-cancellation-of-pressure-drag"></a>
![](cylinder-pressure-taps-ideal-coefficient.png)

**[Figure 4](#image-ideal-cylinder-pressure-coefficients-pressure-tapping-and-cancellation-of-pressure-drag). Ideal cylinder pressure coefficients, pressure tapping and cancellation of pressure drag**. Original [potential flow around a circular cylinder](fluid-mechanics.md#potential-flow-around-a-circular-cylinder) with zero [circulation](vorticity.md#circulation-physics), not experimental data or a fit. [Angle](geometry-and-topology.md#angle) is measured counterclockwise from the downstream direction. Hollow circles mark sampling locations; arrows show only the reference-subtracted [pressure](pressure.md) [force](force.md) per unit [area](differential-geometry.md#surface-area). A separate [pressure tapping](#pressure-tapping) measures [static pressure](fluid-mechanics.md#static-pressure), rather than [stagnation pressure](fluid-mechanics.md#stagnation-pressure). The front and rear ideal [pressure](pressure.md) [forces](force.md) cancel, so this model predicts zero [drag](fluid-mechanics.md#drag-physics).

For [potential flow around a circular cylinder](fluid-mechanics.md#potential-flow-around-a-circular-cylinder) of radius $a$ with zero [circulation](vorticity.md#circulation-physics), the surface tangential [velocity](classical-mechanics.md#velocity) is $u_\theta=-2U_\infty\sin\theta$. Thus the ideal [pressure coefficient](#pressure-coefficient) is

$$
C_p(\theta)=1-4\sin^2\theta.
$$

With $\theta$ measured from downstream, the front is at $\pi$ and the rear at zero. Both ideal [stagnation points](fluid-mechanics.md#stagnation-point) have $C_p=1$, while the sides at $\pi/2$ and $3\pi/2$ have $C_p=-3$. This exact model is a useful baseline for an experiment; its complete rearward [pressure](pressure.md) recovery is not a prediction for a separated real [fluid wake](fluid-mechanics.md#wake-physics).

To obtain a [force](force.md), integrate the local normal contributions with their directions. Let $\mathbf n$ be the unit [normal vector](differential-geometry.md#normal-vector) from the body into the [fluid](fluid-mechanics.md#fluid) and $\Sigma$ its closed wetted surface:

$$
\mathbf F_p=-\int_\Sigma p\mathbf n\,dA
=-q_\infty\int_\Sigma C_p\mathbf n\,dA,
\qquad \int_\Sigma\mathbf n\,dA=\mathbf0.
$$

The second equality removes a spatially constant reference [pressure](pressure.md) over the closed surface; it does not remove a nonuniform [hydrostatic pressure](fluid-mechanics.md#hydrostatic-pressure) or justify dropping the reference term on an isolated open patch. A negative $C_p$ contributes outwards in this reference-subtracted calculation, even though a positive [absolute pressure](fluid-mechanics.md#absolute-pressure) still pushes inwards locally. Project $\mathbf F_p$ onto the chosen [lift](lift-force.md) and [drag](fluid-mechanics.md#drag-physics) directions. The full [fluid](fluid-mechanics.md#fluid) [force](force.md) also includes $\int_\Sigma\boldsymbol\sigma_{\rm visc}\mathbf n\,dA$ from the [viscous stress tensor](dynamic-viscosity.md#viscous-stress-tensor), including tangential [shear stress](viscous-fluid-flow.md#shear-stress); [pressure tapping](#pressure-tapping) does not measure that contribution.

For the two-dimensional cylinder, [force](force.md) per unit span follows from $dA=a\,d\theta$ per unit span and $\mathbf n=(\cos\theta,\sin\theta)$:

$$
(D'_p,L'_p)=-q_\infty a\int_0^{2\pi}C_p(\theta)(\cos\theta,\sin\theta)\,d\theta.
$$

Substituting $C_p=1-4\sin^2\theta$ gives $(0,0)$: opposite points have identical [pressure coefficients](#pressure-coefficient) and opposite [normal vectors](differential-geometry.md#normal-vector). Zero [drag](fluid-mechanics.md#drag-physics) despite a strongly nonuniform [pressure](pressure.md) is the instructive limitation associated with [D'Alembert's paradox](fluid-mechanics.md#d-alembert-s-paradox). Real [viscosity](dynamic-viscosity.md), [boundary layers](continuum-mechanics.md#boundary-layer) and [flow separation](continuum-mechanics.md#flow-separation) can prevent rearward [pressure](pressure.md) recovery and produce [pressure drag](fluid-mechanics.md#pressure-drag). Thus the measured curve can test the model and estimate a [pressure](pressure.md) contribution without proving that total [drag](fluid-mechanics.md#drag-physics) vanishes.

A motivating measurement is Virginia Tech's [Experiment 3 - Flow Past a Circular Cylinder](physics-bibliography.md#aoe-3054-laboratory-manual/experiment-3-flow-past-a-circular-cylinder). Its open-jet [wind tunnel](fluid-mechanics.md#wind-tunnel) holds a rotatable $140\,\mathrm{mm}$ cylinder with end plates and 36 one-millimetre [pressure tappings](#pressure-tapping) at ten-degree intervals. A reference [Pitot-static tube](fluid-mechanics.md#pitot-static-tube) supplies $p_{0\infty}$ and $p_\infty$ to one digital [manometer](fluid-mechanics.md#manometer); a second connects a surface tap to its positive port and reference [static pressure](fluid-mechanics.md#static-pressure) to its negative port. Record the simultaneous readings:

$$
\Delta p_{\rm ref}=p_{0\infty}-p_\infty,\qquad
\Delta p_i=p_i-p_\infty,\qquad
C_{p,i}=\frac{\Delta p_i}{\Delta p_{\rm ref}}.
$$

The last equality uses the low-speed stopping relation, not an additional [speed](classical-mechanics.md#speed) measurement. The manual requires sealed tubing and zero checks with the tunnel off. It also provides a water-column [manometer](fluid-mechanics.md#manometer): read each column's initial level, and subtract the independently measured reference-to-atmosphere [pressure](pressure.md) from the tap-to-atmosphere readings. Record tap positions after rotation. Compare the two instruments and check spanwise uniformity; end plates do not guarantee two-dimensional flow. [Experiment 3 - Flow Past a Circular Cylinder](physics-bibliography.md#aoe-3054-laboratory-manual/experiment-3-flow-past-a-circular-cylinder)

The inferential distinction matters: the [manometers](fluid-mechanics.md#manometer) directly measure [pressure](pressure.md) differences, the ratio estimates [pressure coefficients](#pressure-coefficient), and a [surface integral](multivariable-calculus.md#surface-integral) estimates the pressure part of the [force](force.md). Measure room [absolute pressure](fluid-mechanics.md#absolute-pressure) and [temperature](temperature.md) if converting the reference difference to [speed](classical-mechanics.md#speed) through the [ideal gas law](ideal-gas.md#ideal-gas-law) $\rho=p_{\rm abs}/(RT)$; use [thermodynamic temperature](second-law-of-thermodynamics.md#thermodynamic-temperature) in that equation. For [force](force.md) reconstruction, cover the complete contour and use [numerical integration](numerical-integration.md) with the tap geometry. Finite tap spacing, unknown end effects, probe disturbance and fluctuations limit that reconstruction; tubes and instruments also average or delay changing [pressures](pressure.md). Retain the signed raw readings, repeated readings and reference readings so that these limits can be assessed. A small reference difference magnifies any zero error in the ratio, rather than producing a reliably large $C_p$.

### Pressure tapping

↑ **Parent:** [Pressure coefficient](#pressure-coefficient)

A small flush opening communicating the local surface [static pressure](fluid-mechanics.md#static-pressure) through tubing to a [manometer](fluid-mechanics.md#manometer) or [pressure transducer](fluid-mechanics.md#pressure-transducer). An upstream-facing [Pitot tube](fluid-mechanics.md#pitot-tube) instead brings incident flow to rest to measure [stagnation pressure](fluid-mechanics.md#stagnation-pressure).

## ↑ Ancestors (4)

1. [Fluid mechanics](fluid-mechanics.md)
2. [Branches of physics](physics.md#branches-of-physics)
3. [Physics](physics.md)
4. [Codex Wiki](README.md)

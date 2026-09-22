# Airfoil

↑ **Parent:** [Fluid mechanics](fluid-mechanics-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Airfoil)

An [airfoil](airfoil.md) (British spelling: [aerofoil](airfoil.md)) is the cross-sectional profile of a lifting surface, such as a wing or blade. Its chord is the straight segment from leading edge to trailing edge, with length $c$; its mean camber line runs midway between its upper and lower surfaces, and its thickness measures their separation. Camber is the departure of that mean line from the chord. The [angle of attack](angle-of-attack.md) describes the profile's orientation relative to the incoming flow. These independent choices let a designer alter the distribution of [pressure](pressure-split.md), [lift](lift-force-split.md) and [drag](drag-physics.md), rather than simply enlarging the surface. [NASA Glenn, Wing Geometry, Airfoil Geometry subsection](https://www1.grc.nasa.gov/beginners-guide-to-aeronautics/wing-geometry/)

The distinction between an [airfoil](airfoil.md) and a finite wing matters. A two-dimensional section model assumes no variation along span and predicts [lift](lift-force-split.md) per unit span $L'$. A wing of span $b$ has a spanwise distribution $L'(z)$ and total [lift](lift-force-split.md) $L=\int_{-b/2}^{b/2}L'(z)\,dz$. Its tip flow and trailing [vortices](phase-vortex.md) generate a downward induced [velocity](velocity.md), called downwash, which changes the local flow seen by the sections. Thus one cannot generally multiply the isolated two-dimensional $L'$ by $b$. The wing aspect ratio $b^2/S$ measures its span relative to its reference area and helps characterize these three-dimensional effects. [James F. Marchman III, Aerodynamics and Aircraft Performance, chapter 3.4: finite wings](https://pressbooks.lib.vt.edu/aerodynamics/chapter/chapter-3-additional-aerodynamic-tools/)

For a thin section with small camber slopes and small [angle of attack](angle-of-attack.md), [thin airfoil theory](thin-airfoil-theory.md) predicts

$$
c_l\simeq2\pi(\alpha-\alpha_{L=0}),\qquad
\frac{dc_l}{d\alpha}\simeq2\pi,
$$

where both [angles](angle.md) are in [radians](radian.md) and $\alpha_{L=0}$ is the zero-lift [angle of attack](angle-of-attack.md). The model assumes two-dimensional, [steady flow](steady-flow.md), [incompressible flow](incompressible-flow.md), [inviscid flow](inviscid-flow.md), an attached outer flow, and smooth departure at a sharp trailing edge (the Kutta condition). This last condition selects the [circulation](circulation-physics.md) used by the [Kutta–Joukowski theorem](kutta-joukowski-theorem.md); with counterclockwise [circulation](circulation-physics.md) $\Gamma$ positive and $\mathbf U_\infty=U_\infty\mathbf e_x$, that theorem gives $L'=-\rho_\infty U_\infty\Gamma$ for positive lift towards $+\mathbf e_y$. The beauty is that a detailed [velocity field](velocity-field.md) collapses to a simple force law, while the geometry enters through $\alpha_{L=0}$. [MIT Unified Engineering, F3 lecture notes, pp. 2–4: camber and lift slope](https://ocw.mit.edu/courses/16-01-unified-engineering-i-ii-iii-iv-fall-2005-spring-2006/d721171c42af48a056aaccec784a6d10_f03_0304.pdf) [MIT Unified Engineering, F2 questions 7 and 9: symmetric sections and Kutta condition](https://ocw.mit.edu/courses/16-01-unified-engineering-i-ii-iii-iv-fall-2005-spring-2006/cc3f20c40c9451bde6a595fdd96a7e9e_f02_mud_0304.pdf)

A symmetric [airfoil](airfoil.md) has $\alpha_{L=0}=0$ in this model: at $\alpha=4\,{}^\circ=\pi/45$ the predicted [lift coefficient](lift-coefficient.md) is $c_l\simeq0.439$, and reversing $\alpha$ reverses [lift](lift-force-split.md). A stipulated cambered section with $\alpha_{L=0}=-2\,{}^\circ$ instead predicts $c_l\simeq0.219$ at zero [angle of attack](angle-of-attack.md). These are ideal calculations, not measurements or guarantees for a particular profile. Air parcels on the upper and lower surfaces have no obligation to arrive together at the trailing edge; the [pressure](pressure-split.md) and [velocity field](velocity-field.md) must satisfy the flow problem. A symmetric lifting section already makes an unequal-path-length explanation inadequate. [NASA Glenn, Bernoulli and Newton: the equal-transit explanation is incorrect](https://www1.grc.nasa.gov/beginners-guide-to-aeronautics/bernoulli-and-newton/)

Real [airfoils](airfoil.md) have a viscous [boundary layer](boundary-layer.md), even when [inviscid flow](inviscid-flow.md) approximates the outer motion. At sufficiently demanding incidence, [flow separation](flow-separation.md) can become extensive and the [lift coefficient](lift-coefficient.md) departs from its approximately linear law, reaches a maximum and may fall: this is [aerodynamic stall](aerodynamic-stall.md). [Lift](lift-force-split.md) does not generally vanish at [aerodynamic stall](aerodynamic-stall.md). The onset depends on profile, [Reynolds number](reynolds-number.md), surface condition and motion history; $2\pi(\alpha-\alpha_{L=0})$ predicts neither a universal stall angle nor post-stall behavior. The pressure/balance experiment in [lift](lift-force-split.md) makes this limit observable by measuring changes in the surface [pressure](pressure-split.md) distribution alongside the total [force](force-split.md). [James F. Marchman, chapter 3.3: separation invalidates thin-airfoil assumptions](https://pressbooks.lib.vt.edu/aerodynamics/chapter/chapter-3-additional-aerodynamic-tools/)

**Table of contents**

- [Angle of attack](angle-of-attack.md)
- [Thin airfoil theory](thin-airfoil-theory.md)
- [Aerodynamic stall](aerodynamic-stall.md)

## ↑ Ancestors (4)

1. [Fluid mechanics](fluid-mechanics-split.md)
2. [Branches of physics](branches-of-physics.md)
3. [Physics](physics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Aerodynamic stall](aerodynamic-stall.md)
- [Airfoil](airfoil.md)
- [Angle of attack](angle-of-attack.md)
- [Lift coefficient](lift-coefficient.md)
- [Lift (force)](lift-force-split.md)
- [Thin airfoil theory](thin-airfoil-theory.md)

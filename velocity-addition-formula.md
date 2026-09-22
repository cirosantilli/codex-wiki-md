# Velocity-addition formula

↑ **Parent:** [Lorentz transformation](lorentz-transformation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Velocity-addition_formula)

The [velocity-addition formula](velocity-addition-formula.md) translates a particle's [velocity](velocity.md) between two specified [inertial frames](inertial-frame.md). Let $S'$ move at signed [velocity](velocity.md) $V$ along the $x$-axis of $S$, with parallel axes and $|V|<c$, where $c$ is the [speed of light](speed-of-light.md). Define $u_x=dx/dt$ and $u'_x=dx'/dt'$ for the same particle's [world line](world-line.md), using position and time measured within the corresponding [inertial frame](inertial-frame.md). With [Lorentz factor](lorentz-factor.md) $\gamma_V=(1-V^2/c^2)^{-1/2}$, the forward [Lorentz boost](lorentz-boost.md) gives

$$
u'_x=\frac{u_x-V}{1-Vu_x/c^2},\qquad u'_y=\frac{u_y}{\gamma_V(1-Vu_x/c^2)},\qquad u'_z=\frac{u_z}{\gamma_V(1-Vu_x/c^2)}.
$$

For collinear motion, write $u=u_x$ and $u'=u'_x$. The inverse [velocity-addition formula](velocity-addition-formula.md) is

$$
u=\frac{u'+V}{1+Vu'/c^2}.
$$

This is the composition of the particle's [velocity](velocity.md) in $S'$ and that frame's [velocity](velocity.md) relative to $S$. The [velocities](velocity.md) must belong to this same chain of [reference frames](reference-frame.md), with directions specified. Two arbitrary quoted speeds cannot be inserted blindly. Each [velocity](velocity.md) measurement uses distances and clocks in a single [inertial frame](inertial-frame.md), with [Einstein synchronisation](einstein-synchronisation.md) for separated clocks.

For example, let $V=0.6c$ and let the particle travel at $u'=0.6c$ in $S'$. Its [velocity](velocity.md) in $S$ is

$$
u=\frac{0.6c+0.6c}{1+0.6\times0.6}=\frac{15}{17}c\approx0.88235294c.
$$

The [Galilean transformation](galilean-transformation.md) would instead give $u=u'+V=1.2c$, which fails here. For [light](light.md) moving along the positive axis, $u'=c$ gives $u=c$; $u'=-c$ similarly gives $u=-c$. Negative directions also work for massive particles: at $V=0.6c$, $u'=-0.6c$ gives $u=0$, while $u'=-0.8c$ gives $u=-5c/13$. Thus “addition” means composition of signed [velocities](velocity.md), rather than addition of their magnitudes.

<a id="image-relativistic-velocity-addition"></a>
![](relativistic-velocity-addition.png)

**[Figure 6](#image-relativistic-velocity-addition). Relativistic and Galilean velocity composition for a frame moving at 0.6 times the speed of light**. The horizontal coordinate is the particle's [velocity](velocity.md) in $S'$, and the vertical coordinate is its [velocity](velocity.md) in $S$. The [velocity-addition formula](velocity-addition-formula.md) maps $-1<u'/c<1$ into $-1<u/c<1$; the endpoint values $\pm1$ describe [light](light.md). The marked example is $u'/c=0.6$, giving $u/c=15/17$.

A short derivation differentiates the [Lorentz transformation](lorentz-transformation.md): $dx'=\gamma_V(dx-Vdt)$ and $dt'=\gamma_V(dt-Vdx/c^2)$. Dividing these differentials gives the longitudinal [velocity-addition formula](velocity-addition-formula.md). The transverse formulas use $dy'=dy$ and $dz'=dz$, but the same transformed time denominator; omitting it would ignore the [relativity of simultaneity](relativity-of-simultaneity.md). Replacing $V$ by $-V$ gives the inverse. When both relative and particle [velocities](velocity.md) are small compared with the [speed of light](speed-of-light.md), the denominator is close to one and the [nonrelativistic limit](nonrelativistic-limit.md) recovers the [Galilean transformation](galilean-transformation.md).

The formula lets us compare particle motion in a moving apparatus and a laboratory without losing the invariant [speed of light](speed-of-light.md). Einstein's 1905 paper derives the coordinate change in §3 and the composition of [velocities](velocity.md) in §5, including the collinear formula, its light-speed case, and composition of parallel transformations. [Albert Einstein, On the Electrodynamics of Moving Bodies (1905), §§3 and 5; English translation by W. Perrett and G. B. Jeffery, electronic edition by John Walker](https://www.fourmilab.ch/etexts/einstein/specrel/www/). The [rapidity](rapidity.md) parametrization makes the collinear composition particularly simple.

## ↑ Ancestors (5)

1. [Lorentz transformation](lorentz-transformation.md)
2. [Special relativity](special-relativity-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ib/paper-3/10d/solution.md)
- [Rapidity](rapidity.md)
- [Velocity-addition formula](velocity-addition-formula.md)

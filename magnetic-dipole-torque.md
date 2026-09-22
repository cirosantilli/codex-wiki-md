# Magnetic dipole torque

↑ **Parent:** [Magnetic dipole moment](magnetic-dipole-moment.md)

An externally imposed [magnetic field](magnetic-field-split.md) that is nearly uniform over a rigid [current loop](current-loop.md) produces the [torque](torque.md)

$$
\boldsymbol\tau=\mathbf m\times\mathbf B_{\mathrm{ext}},
\qquad
U=-\mathbf m\cdot\mathbf B_{\mathrm{ext}}=-mB\cos\theta.
$$

The [angle](angle.md) $\theta$ is measured between the [magnetic dipole moment](magnetic-dipole-moment.md) and the external [magnetic field](magnetic-field-split.md), not between the plane of the [current loop](current-loop.md) and the [magnetic field](magnetic-field-split.md). The [magnetic dipole potential energy](magnetic-dipole-potential-energy.md) uses a [dot product](dot-product.md), whereas the [torque](torque.md) uses a [cross product](cross-product.md). The [torque](torque.md) is largest when the [magnetic dipole moment](magnetic-dipole-moment.md) is perpendicular to the [magnetic field](magnetic-field-split.md); parallel alignment minimizes the [potential energy](potential-energy.md).[§11.5, equations 11.22–11.23: vector torque and orientation energy](university-physics-volume-2-by-samuel-j-ling-and-others/11-5-force-and-torque-on-a-current-loop.md)

For the sign convention $\mathbf B_{\mathrm{ext}}=B\widehat{\mathbf x}$ and $\mathbf m=m(\cos\theta\widehat{\mathbf x}+\sin\theta\widehat{\mathbf y})$, positive rotation increases $\theta$ and

$$
\tau_z=-mB\sin\theta=-\frac{dU}{d\theta}.
$$

Thus at $0<\theta<\pi$ the [torque](torque.md) turns the [magnetic dipole moment](magnetic-dipole-moment.md) toward the external [magnetic field](magnetic-field-split.md). Both parallel and antiparallel alignment have zero [torque](torque.md), but they are respectively a [stable equilibrium](stable-equilibrium.md) and an [unstable equilibrium](unstable-equilibrium.md). With no [damping](damping.md), a freely released [current loop](current-loop.md) can undergo [oscillation](oscillation.md) around the [stable equilibrium](stable-equilibrium.md); settling requires [damping](damping.md).

<a id="image-angular-potential-energy-and-signed-torque-of-a-magnetic-dipole-in-an-imposed-field"></a>
![](magnetic-dipole-angular-energy-torque.png)

**[Figure 15](#image-angular-potential-energy-and-signed-torque-of-a-magnetic-dipole-in-an-imposed-field). Angular potential energy and signed torque of a magnetic dipole in an imposed field**. The ideal model has $U/(mB)=-\cos\theta$ and $\tau_z/(mB)=-\sin\theta$. The diagram fixes the external [magnetic field](magnetic-field-split.md) along positive $x$, so the [torque](torque.md) is clockwise for the illustrated positive [angle](angle.md). These curves are calculated, not measured data.

In the twelve-turn example, take $B=0.020\,\mathrm T$ and $\theta=60\degree$. The predicted [torque](torque.md) is $\tau_z=-2.35\times10^{-4}\,\mathrm{N\,m}$ and the [magnetic dipole potential energy](magnetic-dipole-potential-energy.md) is $U=-1.36\times10^{-4}\,\mathrm J$. The unit check is $(\mathrm{A\,m^2})\mathrm T=\mathrm{N\,m}=\mathrm J$; [torque](torque.md) and [energy](energy-split.md) have the same [physical dimensions](physical-dimension.md) but different physical meanings.

A short derivation starts with the [magnetic force on a current-carrying wire](magnetic-force-on-a-current-carrying-wire.md), $d\mathbf F=I\,d\mathbf r\times\mathbf B_{\mathrm{ext}}$. In an exactly uniform [magnetic field](magnetic-field-split.md), the net [force](force-split.md) is $I(\oint_Cd\mathbf r)\times\mathbf B_{\mathrm{ext}}=0$, but its [torque](torque.md) need not vanish: opposite sides produce a turning [couple](couple-mechanics.md). Integrating $\mathbf r\times d\mathbf F$ gives $\mathbf m\times\mathbf B_{\mathrm{ext}}$. Integrating $dU=-\tau_z\,d\theta$ at fixed $m$ and $B$ gives the orientation [potential energy](potential-energy.md). This is the mechanical orientation [potential energy](potential-energy.md) for a maintained [electric current](electric-current.md), with the external source held fixed; the [energy](energy-split.md) accounting for field and power supply is a separate problem. A varying external [magnetic field](magnetic-field-split.md) requires corrections across a finite [current loop](current-loop.md), and can also give a net [force](force-split.md).

**Table of contents**

- [Current-loop torque experiment](current-loop-torque-experiment.md)
  - [Torsion dynamometer](torsion-dynamometer.md)

## ↑ Ancestors (6)

1. [Magnetic dipole moment](magnetic-dipole-moment.md)
2. [Magnetic vector potential](magnetic-vector-potential.md)
3. [Electromagnetism](electromagnetism-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Einstein-de Haas effect](einstein-de-haas-effect.md)
- [Einstein-de Haas experiment](einstein-de-haas-experiment.md)

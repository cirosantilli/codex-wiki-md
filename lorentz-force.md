# Lorentz force

↑ **Parent:** [Electromagnetic field tensor](electromagnetic-field-tensor.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lorentz_force)

The [Lorentz force](lorentz-force.md) is the [force](force.md) exerted by an [electric field](electric-field.md) $\mathbf E$ and a [magnetic field](magnetic-field.md) $\mathbf B$ on a body with [electric charge](electric-charge.md) $q$ and [velocity](velocity.md) $\mathbf v$. In [SI](international-system-of-units.md) units its form in nonrelativistic [classical mechanics](classical-mechanics-split.md), using [mass](mass.md) $m$ and [Newton's second law](newton-s-second-law.md), is

$$
\mathbf F=q(\mathbf E+\mathbf v\times\mathbf B),\qquad
m\frac{d\mathbf v}{dt}=q(\mathbf E+\mathbf v\times\mathbf B).
$$

Both fields are evaluated at the body's [position](position.md) at the current [time](time-in-physics.md). The [electric field](electric-field.md) contributes $q\mathbf E$ even at rest, whereas the magnetic [force](force.md) depends on [velocity](velocity.md) through a [cross product](cross-product.md). [OpenStax, electric force and field](https://openstax.org/books/university-physics-volume-2/pages/5-4-electric-field); [OpenStax, magnetic force on moving charge](https://openstax.org/books/university-physics-volume-2/pages/11-2-magnetic-fields-and-lines).

For a concrete [charged particle in a uniform magnetic field](charged-particle-in-a-uniform-magnetic-field.md), use [nondimensionalization](nondimensionalization.md) to stipulate $m=q=B=1$, [magnetic field](magnetic-field.md) $\mathbf B=(0,0,1)$, zero [electric field](electric-field.md), initial [position](position.md) $(0,0,0)$, and initial [velocity](velocity.md) $(1,0,0)$. These are rescaled quantities, not an assertion that the [mass](mass.md), [electric charge](electric-charge.md), and [magnetic field](magnetic-field.md) have the same physical units. At the start, $(1,0,0)\times(0,0,1)=(0,-1,0)$, so the magnetic [acceleration](acceleration.md) points toward $-y$. The resulting [circular motion](circular-motion.md) is

$$
\mathbf r(t)=(\sin t,\cos t-1,0),\qquad
\mathbf v(t)=(\cos t,-\sin t,0),\qquad
\mathbf a(t)=(-\sin t,-\cos t,0).
$$

At $t=\pi/2$ the [position](position.md) is $(1,-1,0)$ and the [velocity](velocity.md) is $(0,-1,0)$; at $t=\pi$ the [position](position.md) is $(0,-2,0)$ and the [velocity](velocity.md) is $(-1,0,0)$. Thus the [circle](circle.md) has center $(0,-1,0)$ and [radius](radius.md) one. Viewed from $+z$ toward the $xy$ [plane](plane.md), the motion is clockwise. Changing only the [electric charge](electric-charge.md) to $q=-1$ gives [position](position.md) $(\sin t,1-\cos t,0)$ and reverses the bending to counterclockwise.

<a id="image-lorentz-force-circular-motion-and-a-helix-in-the-same-uniform-magnetic-field"></a>
![](lorentz-force-orbits.png)

**[Figure 52](#image-lorentz-force-circular-motion-and-a-helix-in-the-same-uniform-magnetic-field). Lorentz force: circular motion and a helix in the same uniform magnetic field**. Stipulated rescaled $m=q=B=1$ and zero [electric field](electric-field.md). Left: positive [electric charge](electric-charge.md) follows the clockwise [circle](circle.md) from initial [velocity](velocity.md) $(1,0,0)$; the [velocity](velocity.md) is tangent and the magnetic [force](force.md) points inward. Dots denote a [magnetic field](magnetic-field.md) out of the [plane](plane.md). Right: adding parallel [velocity](velocity.md) $v_z=0.5$ gives [helical motion in a uniform magnetic field](helical-motion-in-a-uniform-magnetic-field.md), with [position](position.md) $z=0.5t$ and the same transverse [radius](radius.md) one. Straight arrows show [magnetic field lines](magnetic-field-line.md), distinct from the curved path.

Adding initial [velocity](velocity.md) $v_z=0.5$ leaves the transverse [circular motion](circular-motion.md) unchanged and gives

$$
\mathbf r(t)=(\sin t,\cos t-1,0.5t),\qquad
\mathbf v(t)=(\cos t,-\sin t,0.5).
$$

This is a [helix](helix.md) of transverse [radius](radius.md) one, [cyclotron frequency](cyclotron-frequency.md) $\omega_c=1$, and transverse [period](period-of-a-function.md) $T=2\pi$; the advance along $z$ in one turn is $\pi$. The parallel component of [velocity](velocity.md) stays constant because the magnetic [force](force.md) has no parallel component: there is no magnetic [acceleration](acceleration.md) along the [magnetic field](magnetic-field.md). If the initial [velocity](velocity.md) were entirely parallel to the [magnetic field](magnetic-field.md), the magnetic [force](force.md) would vanish and the path would be straight. [OpenStax, circular and helical motion](https://openstax.org/books/university-physics-volume-2/pages/11-3-motion-of-a-charged-particle-in-a-magnetic-field).

More generally, with zero [electric field](electric-field.md), no other [forces](force.md), and a uniform constant [magnetic field](magnetic-field.md) of magnitude $B>0$, decompose [velocity](velocity.md) into perpendicular and parallel components. For nonzero [electric charge](electric-charge.md) $q$, the perpendicular [speed](speed.md) $v_\perp$ determines the [gyroradius](gyroradius.md), while the [cyclotron frequency](cyclotron-frequency.md) is an [angular frequency](angular-frequency.md):

$$
r=\frac{mv_\perp}{|q|B},\qquad
\omega_c=\frac{|q|B}{m},\qquad
T=\frac{2\pi}{\omega_c}=\frac{2\pi m}{|q|B}.
$$

These are nonrelativistic formulas; see the [relativistic cyclotron orbit](relativistic-cyclotron-orbit.md) for the correction. The beauty is that increasing perpendicular [speed](speed.md) increases the [radius](radius.md) in exactly the proportion needed to leave the [period](period-of-a-function.md) unchanged. Conversely, known [magnetic field](magnetic-field.md), perpendicular [speed](speed.md), and measured [radius](radius.md) determine the magnitude of the [electric charge](electric-charge.md) divided by [mass](mass.md). This makes the same geometry useful for comparing bodies with different [electric charge](electric-charge.md) and [mass](mass.md).

Two short checks explain the result. First, the [cross product](cross-product.md) gives $\mathbf v\times\mathbf B=(-\sin t,-\cos t,0)$ for both stipulated positive-[electric charge](electric-charge.md) paths, exactly their [acceleration](acceleration.md). Second, the transverse magnetic [force](force.md) supplies the [centripetal acceleration](centripetal-acceleration.md), so $mv_\perp^2/r=|q|v_\perp B$; for $v_\perp>0$ this gives the [gyroradius](gyroradius.md), and $\omega_c=v_\perp/r$ gives the [cyclotron frequency](cyclotron-frequency.md).

[Magnetic forces do no work](magnetic-forces-do-no-work.md): the instantaneous [power](power.md) of the magnetic part of the [Lorentz force](lorentz-force.md) vanishes because a [cross product](cross-product.md) is perpendicular to its first argument. The [work-energy theorem](work-energy-theorem.md) therefore gives

$$
\frac{dK}{dt}=\mathbf F\cdot\mathbf v
=q\mathbf E\cdot\mathbf v
+q\mathbf v\cdot(\mathbf v\times\mathbf B)
=q\mathbf E\cdot\mathbf v,
\qquad K=\tfrac12m|\mathbf v|^2.
$$

The [dot product](dot-product.md) $\mathbf v\cdot(\mathbf v\times\mathbf B)$ is zero at every instant, rather than only after a full turn. With zero [electric field](electric-field.md) and no other [forces](force.md), the [kinetic energy](kinetic-energy.md) and [speed](speed.md) remain constant; the [electric field](electric-field.md) can increase or decrease [kinetic energy](kinetic-energy.md) according to the sign of $q\mathbf E\cdot\mathbf v$. In the two stipulated examples the constant [kinetic energy](kinetic-energy.md) is respectively $K=1/2$ and $K=5/8$ in rescaled units. The extra parallel [velocity](velocity.md) raises [kinetic energy](kinetic-energy.md) without changing the [gyroradius](gyroradius.md) or the [cyclotron frequency](cyclotron-frequency.md).

For an electric example in rescaled units, stipulate $m=q=1$, zero [magnetic field](magnetic-field.md), constant [electric field](electric-field.md) $\mathbf E=(2,0,0)$, no other [forces](force.md), and rest at $t=0$. The [Lorentz force](lorentz-force.md) gives [acceleration](acceleration.md) $(2,0,0)$ and [velocity](velocity.md) $(2t,0,0)$, hence [kinetic energy](kinetic-energy.md) $K=2t^2$ and [power](power.md) $dK/dt=4t=q\mathbf E\cdot\mathbf v$. At $t=1$, the [kinetic energy](kinetic-energy.md) has risen from zero to two: the [electric field](electric-field.md) has done positive [work](work.md).

The existing [electromagnetic field tensor](electromagnetic-field-tensor.md) formulation expresses the same interaction covariantly. For [four-momentum](four-momentum.md) $p^\mu$ and [four-velocity](four-velocity.md) $u^\mu$, using [proper time](proper-time.md) $\tau$, the [Lorentz force law](lorentz-force.md) is

$$
\frac{dp^\mu}{d\tau}=qF^{\mu\nu}u_\nu.
$$

Its spatial and temporal components are

$$
\frac{d\mathbf p}{dt}=q(\mathbf E+\mathbf v\times\mathbf B),
\qquad
\frac{d\mathcal E}{dt}=q\mathbf E\cdot\mathbf v.
$$

**Table of contents**

- [Hall effect](hall-effect.md)
  - [Hall coefficient](hall-coefficient.md)
- [Gyroradius](gyroradius.md)
- [Larmor theorem](larmor-theorem.md)
- [Radial escape in an inverse-radius axial magnetic field](radial-escape-in-an-inverse-radius-axial-magnetic-field.md)
- [Velocity rotation in a time-dependent axial magnetic field](velocity-rotation-in-a-time-dependent-axial-magnetic-field.md)
- [Magnetic forces do no work](magnetic-forces-do-no-work.md)
- [Geometrization of the Lorentz force by an affine connection](geometrization-of-the-lorentz-force-by-an-affine-connection.md)
- [Electric drift in crossed uniform fields](electric-drift-in-crossed-uniform-fields.md)
- [Lorentz four-force](lorentz-four-force.md)
- [Magnetic force on a current-carrying wire](magnetic-force-on-a-current-carrying-wire.md)
- [Relativistic cyclotron orbit](relativistic-cyclotron-orbit.md)
  - [Charged-particle action over one relativistic cyclotron orbit](charged-particle-action-over-one-relativistic-cyclotron-orbit.md)
- [Lorentz force density](lorentz-force-density.md)
- [E-cross-B drift](e-cross-b-drift.md)
- [Relativistic electromagnetic work-energy theorem](relativistic-electromagnetic-work-energy-theorem.md)
- [Coordinate acceleration of a relativistic charged particle](coordinate-acceleration-of-a-relativistic-charged-particle.md)

## ↑ Ancestors (7)

1. [Electromagnetic field tensor](electromagnetic-field-tensor.md)
2. [Electromagnetic four-potential](electromagnetic-four-potential.md)
3. [Relativistic electromagnetism](relativistic-electromagnetism.md)
4. [Electromagnetism](electromagnetism-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (107)

- [Charged-particle conserved quantity from a Killing symmetry](charged-particle-conserved-quantity-from-a-killing-symmetry.md)
- [Conservation of mechanical energy](conservation-of-mechanical-energy.md)
- [Diffusive establishment time of a wound toroidal field](diffusive-establishment-time-of-a-wound-toroidal-field.md)
- [Drude conductivity and Hall experiment](drude-conductivity-and-hall-experiment.md)
- [Dynamo quenching](dynamo-quenching.md)
- [Earth's outer core](earth-s-outer-core.md)
- [Electric charge](electric-charge.md)
- [Electric force](electric-force.md)
- [Electromagnetic braking of a sliding rod](electromagnetic-braking-of-a-sliding-rod.md)
- [Electromagnetic field](electromagnetic-field.md)
- [Electromagnetism](electromagnetism-split.md)
- [Faraday's law of induction](faraday-s-law-of-induction.md)
- [Flux-surface preservation during magnetic-tube expansion](flux-surface-preservation-during-magnetic-tube-expansion.md)
- [Force on a current sheet from the mean magnetic field](force-on-a-current-sheet-from-the-mean-magnetic-field.md)
- [Geodynamo](geodynamo.md)
- [Helical motion in a uniform magnetic field](helical-motion-in-a-uniform-magnetic-field.md)
- [Kaluza-Klein geodesic Lorentz force](kaluza-klein-geodesic-lorentz-force.md)
- [Kinematic magnetic dynamo](kinematic-magnetic-dynamo.md)
- [Larmor theorem](larmor-theorem.md)
- [Lorentz force](lorentz-force.md)
- [Lossless limit of magnetic loop braking](lossless-limit-of-magnetic-loop-braking.md)
- [Magnetic axial angular-momentum invariant](magnetic-axial-angular-momentum-invariant.md)
- [Magnetic field](magnetic-field.md)
- [Magnetic flux concentration](magnetic-flux-concentration.md)
- [Magnetic force on a current-carrying wire](magnetic-force-on-a-current-carrying-wire.md)
- [Magnetic forces do no work](magnetic-forces-do-no-work.md)
- [Magnetohydrodynamic total pressure](magnetohydrodynamic-total-pressure.md)
- [Mass spectrometry](mass-spectrometry.md)
- [Motional electromotive force](motional-electromotive-force.md)
- [Neutral quadrupolar perturbation of a uniform-current toroidal field](neutral-quadrupolar-perturbation-of-a-uniform-current-toroidal-field.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-38/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-38/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-42/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-4/4e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-43/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-43/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-46/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ia/paper-4/9e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ia/paper-4/11a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ib/paper-2/7b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ib/paper-3/7b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-62/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-62/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-62/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-68/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ia/paper-4/9c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ib/paper-2/17h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-75/2/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-75/3/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-76/1/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-76/2/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-4/12c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-70/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-74/3/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-74/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ia/paper-4/10c/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-3/35e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-65/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-2/17b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-2/17b/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-74/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-74/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ia/paper-4/12a/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-4/15e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-58/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ia/paper-4/3b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-3/36b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-59/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-59/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ia/paper-4/9b/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ia/paper-4/3c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ia/paper-4/10c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-57/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-57/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-57/2/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ia/paper-4/3b/vi/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-3/17d/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-314/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-1/35d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-3/35d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-309/3/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-314/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-314/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-316/2/vi/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ia/paper-4/10a/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-1/37d/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ia/paper-4/3c/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-311/2/e/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-2/16d/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-2/16d/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-1/37a/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-1/37a/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-1/8d/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-314/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ib/paper-3/15d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ii/paper-4/36d/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-314/4/c/solution.md)
- [Poynting theorem](poynting-theorem.md)
- [Radial escape in an inverse-radius axial magnetic field](radial-escape-in-an-inverse-radius-axial-magnetic-field.md)
- [Relativistic particle](relativistic-particle.md)
- [Solenoid](solenoid.md)
- [Stellar rotation-activity feedback](stellar-rotation-activity-feedback.md)
- [Tesla (unit)](tesla-unit.md)
- [Theta pinch](theta-pinch.md)
- [Uniform-current toroidal-field curl reduction](uniform-current-toroidal-field-curl-reduction.md)
- [Velocity rotation in a time-dependent axial magnetic field](velocity-rotation-in-a-time-dependent-axial-magnetic-field.md)
- [Viscous regularization of the Taylor constraint](viscous-regularization-of-the-taylor-constraint.md)

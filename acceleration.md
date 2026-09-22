# Acceleration

↑ **Parent:** [Velocity](velocity.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Acceleration)

[Acceleration](acceleration.md) is the [time](time-in-physics.md) [derivative](derivative.md) of [velocity](velocity.md), equivalently the second [derivative](derivative.md) of [position](position.md):

$$
\mathbf a(t)=\frac{d\mathbf v}{dt}=\frac{d^2\mathbf r}{dt^2}.
$$

It is a [vector](vector.md) with [SI](international-system-of-units.md) unit $\mathrm{m/s^2}$. A change in direction produces [acceleration](acceleration.md) even if [speed](speed.md) stays constant. For example, a car rounding a bend at steady [speed](speed.md) needs an inward resultant [force](force.md) by [Newton's second law](newton-s-second-law.md). Thus [acceleration](acceleration.md) does not mean only speeding up. When $v>0$, the [dot product](dot-product.md) gives $dv/dt=\mathbf v\cdot\mathbf a/v$: a perpendicular [acceleration](acceleration.md) changes direction without changing [speed](speed.md) at that instant.

Take counterclockwise [circular motion](circular-motion.md) about the origin with [radius](radius.md) $R=2\,\mathrm m$ and constant [angular speed](angular-speed.md) $\omega=0.5\,\mathrm{rad/s}$. The [position](position.md), [velocity](velocity.md) and [acceleration](acceleration.md) are

$$
\begin{aligned}
\mathbf r(t)&=(R\cos(\omega t),R\sin(\omega t)),\\
\mathbf v(t)&=(-R\omega\sin(\omega t),R\omega\cos(\omega t)),\\
\mathbf a(t)&=(-R\omega^2\cos(\omega t),-R\omega^2\sin(\omega t))=-\omega^2\mathbf r(t).
\end{aligned}
$$

The [speed](speed.md) is $R\omega=1\,\mathrm{m/s}$ throughout, while the inward [centripetal acceleration](centripetal-acceleration.md) has magnitude $R\omega^2=v^2/R=0.5\,\mathrm{m/s^2}$. At the four cardinal points, reached at $t=0,\pi,2\pi,3\pi\,\mathrm s$, the [velocities](velocity.md) in $\mathrm{m/s}$ are $(0,1),(-1,0),(0,-1),(1,0)$; the [accelerations](acceleration.md) in $\mathrm{m/s^2}$ are $(-0.5,0),(0,-0.5),(0.5,0),(0,0.5)$. The [vectors](vector.md) turn together, remaining perpendicular. [Ling, Sanny and Moebs, section 4.4: uniform circular motion](https://openstax.org/books/university-physics-volume-1/pages/4-4-uniform-and-nonuniform-circular-motion)

<a id="image-constant-speed-with-changing-velocity-and-inward-acceleration-at-four-points-of-a-circle"></a>
![](constant-speed-circular-acceleration.png)

**[Figure 16](#image-constant-speed-with-changing-velocity-and-inward-acceleration-at-four-points-of-a-circle). Constant speed with changing velocity and inward acceleration at four points of a circle**.

The proof outline is just two applications of the [chain rule](chain-rule.md) to $\mathbf r(t)$; $\sin^2(\omega t)+\cos^2(\omega t)=1$ then fixes both magnitudes. The usefulness is geometric: turning requires a [force](force.md) even when a [speed](speed.md) reading remains steady, and doubling [speed](speed.md) at fixed [radius](radius.md) quadruples the required [centripetal acceleration](centripetal-acceleration.md). The same mechanism appears in a [circular orbit](circular-orbit.md).

Historically, Newton's _Principia_, Book I, Section II, Proposition IV, relates the inward [forces](force.md) of uniform [circular motion](circular-motion.md) to the squared arcs traversed in equal [times](time-in-physics.md), divided by their [radii](radius.md). In modern notation, its dependence on [speed](speed.md) and [radius](radius.md) is $v^2/R$; Newton presents a geometric argument rather than the coordinate [derivatives](derivative.md) above. [Newton, Principia, Book I, Proposition IV; Motte's 1729 translation](https://en.wikisource.org/wiki/The_Mathematical_Principles_of_Natural_Philosophy_(1729)/Book_1/Section_2)

**Table of contents**

- [Jerk (kinematics)](jerk-kinematics.md)

## ↑ Ancestors (6)

1. [Velocity](velocity.md)
2. [Position](position.md)
3. [Classical mechanics](classical-mechanics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (119)

- [Acceleration](acceleration.md)
- [Acceleration in polar coordinates](acceleration-in-polar-coordinates.md)
- [Apparent-gravity camera frame](apparent-gravity-camera-frame.md)
- [Astrometry](astrometry.md)
- [Centripetal acceleration](centripetal-acceleration.md)
- [Circular-orbit stability for a power-law central force](circular-orbit-stability-for-a-power-law-central-force.md)
- [Classical mechanics](classical-mechanics-split.md)
- [Clock hypothesis](clock-hypothesis.md)
- [Conical pendulum](conical-pendulum.md)
- [Constant of integration](constant-of-integration.md)
- [Constant speed](constant-speed.md)
- [Controllability](controllability.md)
- [Convective acceleration identity](convective-acceleration-identity.md)
- [Curvature](curvature.md)
- [Double integrator](double-integrator.md)
- [Drude model](drude-model.md)
- [Exact tidal acceleration between separated masses](exact-tidal-acceleration-between-separated-masses.md)
- [Free fall in a constant gravitational field](free-fall-in-a-constant-gravitational-field.md)
- [Gauss planetary equation for the semi-major axis](gauss-planetary-equation-for-the-semi-major-axis.md)
- [Gravitational acceleration](gravitational-acceleration.md)
- [Gravitational field](gravitational-field.md)
- [Gravity gradiometry](gravity-gradiometry.md)
- [Gravity magnitude versus tidal gradient](gravity-magnitude-versus-tidal-gradient.md)
- [Hydrostatic balance](hydrostatic-balance.md)
- [Instantaneous power](instantaneous-power.md)
- [Jeans swindle](jeans-swindle.md)
- [Jerk (kinematics)](jerk-kinematics.md)
- [Kinematic pressure](kinematic-pressure.md)
- [Lorentz force](lorentz-force.md)
- [Magnetic field](magnetic-field.md)
- [Newton's second law](newton-s-second-law.md)
- [Newton (unit)](newton-unit.md)
- [Newtonian gravitational potential](newtonian-gravitational-potential.md)
- [Normal component](normal-component.md)
- [Normal force](normal-force.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ia/paper-4/10a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ia/paper-4/12a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ia/paper-4/3a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ia/paper-4/4a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-47/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-4/3e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-43/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ia/paper-4/10a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ia/paper-4/4a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ia/paper-4/9a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-61/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-61/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-66/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ia/paper-4/3c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ia/paper-4/11b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ia/paper-4/11b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ia/paper-4/9b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ia/paper-4/11a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ia/paper-4/3a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-61/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-59/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ia/paper-2/6b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ia/paper-4/10c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ia/paper-4/9c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ia/paper-4/12b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ia/paper-4/3b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ia/paper-4/4b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ia/paper-4/11a/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-3/23i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-3/36d/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-3/36d/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-316/2/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-316/2/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-316/2/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-316/3/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-320/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-320/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-320/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-320/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ia/paper-4/11a/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ia/paper-4/11a/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ia/paper-4/10c/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ia/paper-4/11c/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-316/2/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ia/paper-4/3c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ia/paper-4/9c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-1/16c/a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-3/12e/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-3/12e/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ib/paper-1/11e/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-1/15d/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-3/9d/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ia/paper-4/12b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ib/paper-1/2f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ii/paper-2/38a/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ii/paper-3/36d/solution.md)
- [Pathline](pathline.md)
- [Physical law](physical-law.md)
- [Point-mass tidal stretching and squeezing](point-mass-tidal-stretching-and-squeezing.md)
- [Radial free fall from rest](radial-free-fall-from-rest.md)
- [Radiation pressure on circumplanetary dust](radiation-pressure-on-circumplanetary-dust.md)
- [Reduced mass](reduced-mass.md)
- [Rocket equation](rocket-equation.md)
- [Rocket thrust](rocket-thrust.md)
- [Simple harmonic motion](simple-harmonic-motion.md)
- [Simple pendulum](simple-pendulum.md)
- [Speed-radius attractor of an accreting raindrop](speed-radius-attractor-of-an-accreting-raindrop.md)
- [Static friction](static-friction.md)
- [Stokes settling velocity](stokes-settling-velocity.md)
- [Tangential and normal acceleration](tangential-and-normal-acceleration.md)
- [Tangential component](tangential-component.md)
- [Terminal velocity](terminal-velocity.md)
- [Terminal velocity under linear drag](terminal-velocity-under-linear-drag.md)
- [Tidal disruption](tidal-disruption.md)
- [Tidal force](tidal-force.md)
- [Tidal tensor](tidal-tensor.md)
- [Timelike geodesic](timelike-geodesic.md)
- [Torque criterion for constant areal velocity](torque-criterion-for-constant-areal-velocity.md)
- [Twin paradox clock experiments](twin-paradox-clock-experiments.md)
- [Twin paradox with finite acceleration](twin-paradox-with-finite-acceleration.md)
- [Unsteady Stokes equation](unsteady-stokes-equation.md)
- [Vertical ascent under linear drag](vertical-ascent-under-linear-drag.md)
- [Viscous stress tensor](viscous-stress-tensor.md)
- [Wave equation](wave-equation-split.md)

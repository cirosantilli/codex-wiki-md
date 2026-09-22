<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

**Constraint and example.** A [holonomic constraint](../../../holonomic-constraint.md) can be written $f_\alpha(q_1,\ldots,q_n,t)=0$, with no irreducible dependence on [velocities](../../../velocity.md). A velocity relation is holonomic if it integrates to such an equation. For example, a particle constrained to a stationary circle satisfies $x^2+y^2=\ell^2$, reducing its two Cartesian [degrees of freedom](../../../degree-of-freedom.md) to one angle. A [nonholonomic constraint](../../../nonholonomic-constraint.md) cannot be integrated in this way.

**Kinematics and kinetic energy.** Set $d=R-r>0$. In the plane of the original diagram, choose the orbital angle $\theta$ positive counterclockwise from vertically downward. The marked radius of the inner cylinder then has absolute orientation $\alpha=\theta-\phi$ measured from the same downward direction. Its signed spin [angular velocity](../../../angular-velocity.md) is $\Omega=\dot\theta-\dot\phi$, while

$$
\mathbf X_G=d(\sin\theta,-\cos\theta),\qquad |\dot{\mathbf X}_G|=d|\dot\theta|.
$$

The [moment of inertia of a uniform solid cylinder](../../../moment-of-inertia-of-a-uniform-solid-cylinder.md) is $I=mr^2/2$. Applying the [kinetic energy decomposition about the center of mass](../../../kinetic-energy-decomposition-about-the-center-of-mass.md) gives

$$
\boxed{T=\frac12md^2\dot\theta^2+\frac12I\Omega^2
=\frac m2(R-r)^2\dot\theta^2+\frac m4r^2(\dot\phi-\dot\theta)^2.}
$$

**No slip.** With tangential unit vector $\mathbf e_\theta=(\cos\theta,\sin\theta)$, the inner contact point has [velocity](../../../velocity.md) $(d\dot\theta+r\Omega)\mathbf e_\theta$. The fixed wall requires this to vanish. Hence

$$
d\dot\theta+r(\dot\theta-\dot\phi)=0,\qquad R\dot\theta-r\dot\phi=0.
$$

Because $r,R$ are constant, integration gives

$$
\boxed{r\phi-R\theta=0,\qquad \Omega=-\frac{R-r}{r}\dot\theta,}
$$

where the integration constant is zero with the marked-dot reference in the diagram and continuously unwrapped angles. This is a [holonomic constraint](../../../holonomic-constraint.md), even though it was first obtained from a condition on [velocities](../../../velocity.md).

**Oscillations.** The [gravitational potential energy](../../../gravitational-energy.md) above the lowest position is $V=mgd(1-\cos\theta)$. Eliminating $\phi$ gives the reduced [Lagrangian](../../../lagrangian.md)

$$
L=\frac34md^2\dot\theta^2-mgd(1-\cos\theta).
$$

The [Euler-Lagrange equation](../../../euler-lagrange-equation.md) becomes

$$
\frac32md^2\ddot\theta+mgd\sin\theta=0.
$$

Thus the bottom is a stable equilibrium, and for $|\theta|\ll1$ there is [simple harmonic motion](../../../simple-harmonic-motion.md), with

$$
\boxed{\omega_0=\sqrt{\frac{2g}{3(R-r)}},\qquad
f_0=\frac1{2\pi}\sqrt{\frac{2g}{3(R-r)}}.}
$$

The extra rotational [kinetic energy](../../../kinetic-energy.md) reduces the frequency compared with a particle sliding without friction along the same circular path. The [small oscillations inside a circular cylinder](../../../small-oscillations-inside-a-circular-cylinder.md) formula applies with inertia ratio $\gamma=1/2$.

**Friction and energy.** Let $F_t$ be the signed tangential contact force in the $\mathbf e_\theta$ direction. Applying [Newton's second law](../../../newton-s-second-law.md) to translation and the [torque](../../../torque.md) equation to rotation gives

$$
md\ddot\theta=-mg\sin\theta+F_t,\qquad
I\dot\Omega=rF_t.
$$

Using the [rolling without slipping](../../../rolling-without-slipping.md) condition yields

$$
\boxed{F_t=\frac13mg\sin\theta.}
$$

Except at special instants, [static friction](../../../static-friction.md) is needed to produce the spin acceleration. There is no sliding at the contact point, whose instantaneous [velocity](../../../velocity.md) is zero; therefore this force does no total work. Its translational and rotational powers cancel: $F_td\dot\theta+F_tr\Omega=0$. The stationary [normal reaction](../../../normal-force.md) likewise does no work. With a rigid wall, adequate [static friction](../../../static-friction.md), and no rolling resistance, [conservation of energy](../../../conservation-of-energy.md) gives

$$
\boxed{E=\frac34md^2\dot\theta^2+mgd(1-\cos\theta)=\text{constant}.}
$$

**Angular momentum.** The cylinder's spin [angular momentum](../../../angular-momentum.md) $I\Omega$ is generally not conserved because the contact friction exerts a [torque](../../../torque.md) about its [center of mass](../../../center-of-mass.md). About the fixed outer-cylinder center $O$, the [angular momentum decomposition about the centre of mass](../../../angular-momentum-decomposition-about-the-centre-of-mass.md) gives

$$
L_O=md^2\dot\theta+I\Omega=md\left(d-\frac r2\right)\dot\theta.
$$

Gravity and friction exert the external [torque](../../../torque.md)

$$
\dot L_O=-mgd\sin\theta+RF_t
=mg\left(r-\frac{2R}{3}\right)\sin\theta.
$$

Thus **the rolling cylinder does not generally conserve angular momentum**, although it conserves mechanical [energy](../../../energy-split.md). There is a special geometric cancellation at $R=3r/2$: then $L_O$ and its torque vanish identically for this planar motion. Angular momentum of a larger isolated system including the wall and Earth is a separate conservation statement.

**Scope of the holonomic reduction.** The integrated constraint is exact at every angle for planar [rolling without slipping](../../../rolling-without-slipping.md) with sustained contact; it is not restricted to [small oscillations](../../../small-oscillation.md). Completing a full turn requires tracking angle winding rather than reducing each angle separately modulo $2\pi$. This global bookkeeping does not make the local velocity relation nonintegrable.

However, arbitrary initial conditions need not sustain this ideal rolling motion. The inward [normal reaction](../../../normal-force.md) and the required friction are

$$
N=m(g\cos\theta+d\dot\theta^2),\qquad |F_t|=\frac13mg|\sin\theta|.
$$

Contact requires $N\geq0$, and a finite coefficient $\mu_s$ of [static friction](../../../static-friction.md) requires $|F_t|\leq\mu_sN$. If either fails, the cylinder detaches or slips and the one-coordinate rolling [Lagrangian](../../../lagrangian.md) no longer applies. Slipping contact allows $\theta$ and $\phi$ to be independent; detachment removes the fixed center-distance constraint. These changes alone do not establish a [nonholonomic constraint](../../../nonholonomic-constraint.md). Allowing general three-dimensional reorientation can introduce nonintegrable rolling constraints, but that motion is outside the diagram's two-angle planar model. Thus **the stated planar rolling constraint is holonomic throughout its regime of validity; it cannot be imposed on every physically possible motion**.

## ↑ Ancestors (13)

1. [2](../2.md)
2. [2019](../../2019-split.md)
3. [Past exam of the theoretical physics I course of the University of Cambridge](../../split.md)
4. [Theoretical Physics I course of the University of Cambridge](../../../theoretical-physics-i-course-of-the-university-of-cambridge.md)
5. [Theoretical Physics course of the University of Cambridge](../../../theoretical-physics-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../university-of-cambridge-split.md)
12. [List of universities](../../../list-of-universities.md)
13. [Codex Wiki](../../../split.md)

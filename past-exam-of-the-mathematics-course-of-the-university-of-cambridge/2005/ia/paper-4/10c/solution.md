<h1 id="10c/solution">Solution</h1>

↑ **Parent:** [10C](../10c.md)

The rim-mass wheel has [moment of inertia](../../../../../moment-of-inertia.md) $I=MR^2$. A uniform solid cylinder has axial moment $\tfrac12mS^2$, so the roller of mass $M/2$ has $J=MS^2/4$. No slip gives equal contact speeds, $R\omega=S\sigma$, when $\omega,\sigma$ denote angular-speed magnitudes. Therefore

$$
\boxed{I=MR^2,\quad J=\frac{MS^2}{4},\quad \frac{\sigma}{\omega}=\frac RS.}
$$

With parallel signed axes the two [angular velocities](../../../../../angular-velocity.md) have opposite signs. Their [kinetic energies](../../../../../kinetic-energy.md) add regardless of that convention:

$$
\frac12I\omega^2+\frac12J\sigma^2
=\frac12\left[I+J(R/S)^2\right]\omega^2
=\frac12K\omega^2,\qquad \boxed{K=\frac54MR^2.}
$$

The [reflected inertia of a no-slip wheel and roller](../../../../../reflected-inertia-of-a-no-slip-wheel-and-roller.md) must be used because accelerating the wheel also accelerates the roller. The transmitted contact forces redistribute energy without dissipating it. For an applied wheel [torque](../../../../../torque.md) $T$, the input power is $T\omega$, so the [work-energy theorem](../../../../../work-energy-theorem.md) gives $K\omega\dot\omega=T\omega$, or $K\dot\omega=T$; this also holds at rest by continuity or the constrained equation of motion.

Assume the driving constants $Q,\Omega$ are positive. With the speed-dependent [torque](../../../../../torque.md),

$$
K\dot\omega=Q(1-\omega/\Omega),\qquad\omega(0)=0.
$$

Separating this linear equation gives

$$
\boxed{\omega(t)=\Omega\left(1-e^{-Qt/(K\Omega)}\right).}
$$

For the fan, its resisting roller [torque](../../../../../torque.md) dissipates power $\gamma\sigma^3$. Expressing this in the wheel coordinate gives a resisting wheel torque $\gamma(R/S)^3\omega^2$. Thus, with $\Gamma=\gamma(R/S)^3$,

$$
K\dot\omega=Q(1-\omega/\Omega)-\Gamma\omega^2.
$$

The right-hand side is positive at zero, strictly decreasing for nonnegative $\omega$, and has a unique positive zero; the wheel starting at rest approaches this terminal angular speed. Hence

$$
\boxed{\omega_{{\max}}=\frac{2Q}{Q/\Omega+\sqrt{(Q/\Omega)^2+4\gamma Q(R/S)^3}},\qquad
v_{{\rm rim,max}}=R\omega_{{\max}}.}
$$

For a nonzero fan drag this is less than $\Omega$, and as $\gamma\to0$ it tends to $\Omega$. The cubed radius ratio is essential: one factor arises from converting roller power to wheel torque, in addition to the two factors in $\sigma^2$.

## ↑ Ancestors (10)

1. [10C](../10c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

<h1 id="10b/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Apply the [rotating-frame derivative formula](../../../../../../rotating-frame-derivative-formula.md) first to $r$, then to $v'= [dr/dt]_{S'}$. Since the [angular velocity](../../../../../../angular-velocity.md) is constant in either frame,

$$
\left[\frac{dr}{dt}\right]_S=v'+\omega\times r,
$$



$$
\boxed{\left[\frac{d^2r}{dt^2}\right]_S=\left[\frac{d^2r}{dt^2}\right]_{S'}+2\omega\times v'+\omega\times(\omega\times r).}
$$

The two apparent [forces](../../../../../../force.md) in the rotating equation are the [Coriolis force](../../../../../../coriolis-force.md) and the [centrifugal acceleration](../../../../../../centrifugal-acceleration.md) multiplied by [mass](../../../../../../mass.md). Thus

$$
m\left[\frac{dv'}{dt}\right]_{S'}=-\nabla\phi+G-2m\omega\times v'-m\omega\times(\omega\times r).
$$

Set $\phi_{\rm eff}=\phi-\tfrac m2|\omega\times r|^2$. The supplied gradient identity gives $\nabla\phi_{\rm eff}=\nabla\phi+m\omega\times(\omega\times r)$. Taking the scalar product with $v'$ removes $G$, since it is orthogonal to $v'$, and removes the [Coriolis force](../../../../../../coriolis-force.md). Therefore the [energy balance in a uniformly rotating frame](../../../../../../energy-balance-in-a-uniformly-rotating-frame.md) is

$$
\boxed{\frac{d}{dt}\left(\frac m2|v'|^2+\phi-\frac m2|\omega\times r|^2\right)=\left(\frac{\partial\phi}{\partial t}\right)_{r'}.}
$$

**The displayed quantity is conserved when the potential is stationary in the rotating coordinates.** This includes a static inertial potential invariant under rotations about the chosen axis, such as vertical gravity in part (b). If the word conservative only means a time-independent inertial potential, that extra rotational invariance is needed; a conservative [force](../../../../../../force.md) alone does not imply the claimed conservation.

For an explicit counterexample to that unrestricted interpretation, take unit [mass](../../../../../../mass.md), an inertial [force](../../../../../../force.md) $F=e_x$, $\phi=-x$, no $G$, rotation $\omega=\omega e_z$, and inertial trajectory $r(t)=(t^2/2,1,0)$ with initial [velocity](../../../../../../velocity.md) zero. It satisfies [Newton's second law](../../../../../../newton-s-second-law.md). Substituting $v'=\dot r-\omega\times r$ into the proposed energy gives $E=\omega t$, which is not constant for nonzero rotation. The qualified conservation law above is the one used for the hoop.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [10B](../../10b.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

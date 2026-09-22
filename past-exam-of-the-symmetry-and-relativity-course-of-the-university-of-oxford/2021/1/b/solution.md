<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $\Gamma=(1-v^2/c^2)^{-1/2}$ for the [Lorentz factor](../../../../lorentz-factor.md) of the [inertial frame](../../../../inertial-frame.md) $S'$, distinguishing it from the particles' changing [Lorentz factors](../../../../lorentz-factor.md). Apply the [Lorentz transformation](../../../../lorentz-transformation.md)

$$
x'=\Gamma(x-vt),\qquad t'=\Gamma(t-vx/c^2)
$$

to each [world line](../../../../world-line.md) in [a](../a.md). Both particles initially have [velocity](../../../../velocity.md) $-v$ in $S'$. The switching events have coordinates

$$
(t'_e,x'_e)=(0,0),\qquad
(t'_p,x'_p)=(-\Gamma vd/c^2,\Gamma d).
$$

Thus the [Positron](../../../../positron.md) starts accelerating earlier in $S'$. Its [velocity](../../../../velocity.md) first becomes less negative, vanishes when its laboratory [velocity](../../../../velocity.md) reaches $v$, and then becomes positive. The [electron](../../../../electron.md) continues at $-v$ until $t'=0$, then accelerates toward $-c$. The [relativistic velocity-addition formula](../../../../velocity-addition-formula.md) makes this precise:

$$
u'_e=\frac{u_e-v}{1-vu_e/c^2},\qquad
u'_p=\frac{u_p-v}{1-vu_p/c^2}.
$$

The [electric field](../../../../electric-field-split.md) parallel to the [Lorentz boost](../../../../lorentz-boost.md) has unchanged magnitude, but its switching surface is $t'+vx'/c^2=0$, rather than $t'=0$ everywhere.

In the laboratory, the total [three-momentum](../../../../three-momentum.md) is zero for all $t$: the two [Lorentz forces](../../../../lorentz-force.md) cancel at equal laboratory times. In $S'$, each active force is still $qE$, since this is one-dimensional motion with a parallel [electric field](../../../../electric-field-split.md). Define $t'_p=-\Gamma vd/c^2$. For $v>0$ the total [three-momentum](../../../../three-momentum.md), evaluated at **equal $t'$**, is

$$
\boxed{P'_x(t')=
\begin{cases}
-2\Gamma mv,&t'<t'_p,\\
-2\Gamma mv+F(t'-t'_p),&t'_p\leq t'<0,\\
-2\Gamma mv+\Gamma Fvd/c^2,&t'\geq0.
\end{cases}}
$$

This follows by integrating $dp'_p/dt'=F$ from its switching event and $dp'_e/dt'=-F$ from its later switching event. During the interval between them only the [Positron](../../../../positron.md) feels the prescribed [electric field](../../../../electric-field-split.md), so [momentum conservation](../../../../momentum-conservation.md) for the particle pair fails. Once both forces act, the total [three-momentum](../../../../three-momentum.md) is constant again.

The [equal-time momentum of an externally driven particle pair](../../../../equal-time-momentum-of-an-externally-driven-particle-pair.md) illustrates a distinction. The sum of particle [four-momenta](../../../../four-momentum.md) **at a fixed pair of events** is always a [four-vector](../../../../four-vector.md). However, a fresh sum at equal time in each [inertial frame](../../../../inertial-frame.md) generally uses different events. Here transforming an equal-$t$ laboratory sum would give $-2\Gamma v\sqrt{m^2c^4+F^2c^2t^2}/c^2$, which varies with $t$; this differs from the equal-$t'$ answer above. For example, with $c=m=F=d=1$ and $v=0.6$, the late-time equal-$t'$ sum is $-0.75$, whereas transforming the equal-$t=0$ sum gives $-1.5$. This is a concrete failure of treating the pair's equal-time sums as components of a single frame-independent [four-vector](../../../../four-vector.md).

A closed system's total [four-momentum](../../../../four-momentum.md), including the [electromagnetic field](../../../../electromagnetic-field.md) and the apparatus supplying it, is conserved and independent of the choice of spacelike integration surface under the usual isolated-system boundary conditions. The particles alone exchange [energy](../../../../energy-split.md) and [momentum](../../../../momentum-split.md) with an external system, so neither that independence nor universal particle-only [momentum conservation](../../../../momentum-conservation.md) is guaranteed.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the symmetry and relativity course of the University of Oxford](../../../split.md)
5. [Symmetry and relativity course of the University of Oxford](../../../../symmetry-and-relativity-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

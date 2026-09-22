<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Orient the ring's area normal with positive external [magnetic flux](../../../magnetic-flux.md). [Faraday's law](../../../faraday-s-law-of-induction.md) gives the applied [electromotive force](../../../electromotive-force.md)

$$
\mathcal E_{\rm ext}=-\frac{d}{dt}(AB_0\cos\omega t)
=AB_0\omega\sin\omega t.
$$

The ring's [self-inductance](../../../self-inductance.md) opposes changes in its [electric current](../../../electric-current.md). With positive [electrical resistance](../../../electrical-resistance.md) $R$, [Kirchhoff's voltage law](../../../kirchhoff-cycle-law.md) therefore gives $L\dot I+RI=\mathcal E_{\rm ext}$. Define $\phi=\tan^{-1}(\omega L/R)$. The periodic steady state is

$$
\boxed{I(t)=\frac{AB_0\omega}{\sqrt{R^2+\omega^2L^2}}\sin(\omega t-\phi),\qquad
\langle P\rangle=\frac{R A^2B_0^2\omega^2}{2(R^2+\omega^2L^2)}.}
$$

The second result follows from [Joule heating](../../../joule-heating.md), $P=RI^2$, and $\langle\sin^2\rangle=1/2$. For unspecified initial conditions, add a transient $I_h=C\exp(-Rt/L)$; the displayed time average is over the periodic steady state after that transient has decayed. The [inductor](../../../inductor.md) temporarily stores and returns [energy](../../../energy-split.md), with no net storage change over one complete cycle.

## ↑ Ancestors (11)

1. [2](../2.md)
2. [2017](../../2017-split.md)
3. [Past exam of the physics 2 paper of the University of Oxford](../../split.md)
4. [Physics 2 paper of the University of Oxford](../../../physics-2-paper-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)

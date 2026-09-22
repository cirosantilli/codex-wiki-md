<h1 id="section-c/c10/solution">Solution</h1>

↑ **Parent:** [C10](../c10.md)

After switching, [Kirchhoff's voltage law](../../../../../kirchhoff-cycle-law.md) gives the free [series RLC circuit](../../../../../series-rlc-circuit.md) equation

$$
L\ddot q+R\dot q+q/C=0.
$$

Its characteristic roots are $-\gamma\pm i\omega_d$, where

$$
\boxed{\gamma=\frac R{2L},\qquad \omega_d=\sqrt{\frac1{LC}-\frac{R^2}{4L^2}}.}
$$

A real, nonzero oscillation [frequency](../../../../../frequency.md) requires $R^2<4L/C$. For a passive [resistor](../../../../../resistor.md),

$$
\boxed{0\leq R<2\sqrt{L/C}\simeq894\ \Omega.}
$$

The endpoint $R=0$ is the undamped limit; strictly decaying oscillations have $0<R<894\ \Omega$. The critical endpoint itself does not have a nonzero $\omega_d$.

Let $Q=CV_0$ denote the initial [electric charge](../../../../../electric-charge-split.md), so $Q=30\ \mu\mathrm C$ and $\dot q(0)=0$. Distinguish $Q$ from the amplitude coefficient $q_0$ in an exponential-times-cosine representation: imposing zero initial [electric current](../../../../../electric-current.md) generally requires a nonzero phase.

## ↑ Ancestors (13)

1. [C10](../c10.md)
2. [Section C](../../section-c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2016](../../../split.md)
5. [Past exam of the physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

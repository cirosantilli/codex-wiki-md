<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The expression obtained in part (a)(iii) gives a direct deterministic bound. For every fixed $T<\infty$ and $0\leq s\leq T$,

$$
0<Z_s
=\exp\!\left[\frac{\beta s}{2}-\frac\beta2B_s^2
-\frac{\beta^2}{2}\int_0^sB_u^2du\right]
\leq e^{\beta T/2}.
$$

Thus the [bounded local martingale criterion](../../../../../bounded-local-martingale-criterion.md) makes $Z$ a true [martingale](../../../../../martingale-split.md) on every finite time interval. More explicitly, if $\sigma_n$ is a [localizing sequence](../../../../../localizing-sequence.md), the identities $\mathbb E[Z_{t\wedge\sigma_n}\mid\mathcal F_s]=Z_{s\wedge\sigma_n}$ pass to the limit by [dominated convergence](../../../../../dominated-convergence-theorem.md), using the displayed bound for $t\leq T$. Therefore

$$
\boxed{\mathbb E[Z_t\mid\mathcal F_s]=Z_s,\qquad \mathbb EZ_t=1\quad(0\leq s\leq t<\infty).}
$$

This establishes exactly the finite-horizon property needed for the subsequent change of measure.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the stochastic differential equations course of the University of Oxford](../../../../split.md)
6. [Stochastic differential equations course of the University of Oxford](../../../../../stochastic-differential-equations-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $N_t=M_t-M_0$ and $V_t=\langle M\rangle_t=[N]_t$. The [Dambis-Dubins-Schwarz theorem](../../../../dambis-dubins-schwarz-theorem.md) supplies a standard [Brownian motion](../../../../brownian-motion-split.md) $W$ such that

$$
N_t=W_{V_t}.
$$

On the event $V_\infty=\infty$, continuity and monotonicity imply that the range of $t\mapsto V_t$ is all of $[0,\infty)$.

For completeness, [Brownian motion](../../../../brownian-motion-split.md) hits every positive integer [almost surely](../../../../almost-sure-convergence.md). The [Brownian reflection principle](../../../../reflection-principle-wiener-process.md) gives, for $a>0$,

$$
\mathbb P\!\left(\sup_{0\leq u\leq R}W_u\geq a\right)
=2\mathbb P(W_R\geq a)\longrightarrow1\qquad(R\to\infty).
$$

Intersect over integer $a$. The times of these increasingly large values must escape every compact interval because each Brownian path is continuous there. Therefore $\limsup_{u\to\infty}W_u=\infty$. The unbounded clock transfers these values to arbitrarily late times for $N$, and adding the finite initial value $M_0$ preserves unboundedness. Hence

$$
\boxed{\limsup_{t\to\infty}|M_t|=\infty\quad\text{almost surely}.}
$$

This is an instance of [infinite quadratic variation forces unbounded oscillations](../../../../infinite-quadratic-variation-forces-unbounded-oscillations.md); applying the same argument to $-W$ also gives negative oscillations.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the stochastic differential equations course of the University of Oxford](../../../split.md)
5. [Stochastic differential equations course of the University of Oxford](../../../../stochastic-differential-equations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

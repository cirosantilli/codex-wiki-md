<h1 id="a/3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Fix a finite horizon $T$ and use the completed [natural Brownian filtration](../../../../../natural-brownian-filtration.md). [Martingale representation theorem](../../../../../martingale-representation-theorem.md) states that every $F\in L^2(\mathcal F_T)$ can be written

$$
F=\mathbb EF+\int_0^T H_s\,dB_s,
\qquad \mathbb E\int_0^T H_s^2ds<\infty,
$$

where $H$ is predictable and is unique up to equality for $ds\,d\mathbb P$ almost every $(s,\omega)$.

The [Martingale representation theorem](../../../../../martingale-representation-theorem.md) states that every [square-integrable martingale](../../../../../square-integrable-martingale.md) $M$ in this [filtration](../../../../../filtration-probability-theory.md) has a continuous version of the form

$$
\boxed{M_t=M_0+\int_0^tH_s\,dB_s,\quad0\leq t\leq T,}
$$

with the same integrability and uniqueness condition. The completed natural [filtration](../../../../../filtration-probability-theory.md) has only null-set randomness at time zero, so $M_0$ is almost surely constant. The first statement gives the second by representing $M_T$ and taking [conditional expectations](../../../../../conditional-expectation.md); the second gives the first by taking $M_t=\mathbb E(F\mid\mathcal F_t)$.

There is also the local version: every [local martingale](../../../../../local-martingale.md) in the [Brownian filtration](../../../../../brownian-filtration.md) has a continuous version representable by a predictable, locally square-integrable integrand. The [filtration](../../../../../filtration-probability-theory.md) restriction matters; an enlarged [filtration](../../../../../filtration-probability-theory.md) with independent additional [martingales](../../../../../martingale-split.md) need not have representation using $B$ alone.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [3](../../3.md)
3. [A](../../../a.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../split.md)
6. [Stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../../stochastic-differential-equations-and-brownian-motion-in-complex-analysis-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

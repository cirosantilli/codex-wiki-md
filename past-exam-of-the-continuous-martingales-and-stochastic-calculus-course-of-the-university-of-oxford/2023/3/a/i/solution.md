<h1 id="3/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [optional stopping theorem](../../../../../optional-sampling-theorem-for-a-supermartingale.md) for a right-continuous [martingale](../../../../../martingale-split.md) $M$ on a [filtered probability space](../../../../../filtered-probability-space.md) satisfying the [usual conditions for a filtration](../../../../../usual-conditions-for-a-filtration.md) states that, for bounded [stopping times](../../../../../stopping-time.md) $\sigma\leq\tau$,

$$
\boxed{\mathbb E[M_\tau\mid\mathcal F_\sigma]=M_\sigma,
\qquad \mathbb EM_\tau=\mathbb EM_\sigma.}
$$

For a [submartingale](../../../../../submartingale.md) the conditional equality becomes $\mathbb E[M_\tau\mid\mathcal F_\sigma]\geq M_\sigma$, and for a [supermartingale](../../../../../supermartingale.md) it becomes the reverse inequality.

For a [uniformly integrable martingale](../../../../../uniformly-integrable-martingale.md), boundedness of the [stopping times](../../../../../stopping-time.md) can be removed, with the terminal limit used if a [stopping time](../../../../../stopping-time.md) is infinite. A useful application is to a bounded [stopped martingale](../../../../../stopped-martingale.md) $M_{t\wedge\tau}$ with $\tau<\infty$ [almost surely](../../../../../almost-sure-convergence.md): apply the bounded-time theorem first and then the [bounded convergence theorem](../../../../../bounded-convergence-theorem.md) to obtain $\mathbb EM_\tau=\mathbb EM_0$. Finiteness of $\tau$ alone is not a sufficient hypothesis for an arbitrary [martingale](../../../../../martingale-split.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the continuous martingales and stochastic calculus course of the University of Oxford](../../../../split.md)
6. [Continuous martingales and stochastic calculus course of the University of Oxford](../../../../../continuous-martingales-and-stochastic-calculus-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

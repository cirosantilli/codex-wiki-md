<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Strict positivity lets us define the [continuous local martingale](../../../../../../continuous-local-martingale.md)

$$
\boxed{X_t=\int_0^t\frac{dM_s}{M_s}.}
$$

The integrand is locally bounded because a positive continuous path has positive minimum on every compact time interval. The [Itô formula](../../../../../../ito-s-lemma.md) for $\log M$ gives

$$
\log M_t=X_t-\frac12\langle X\rangle_t,\qquad\boxed{M_t=\exp\left(X_t-\frac12\langle X\rangle_t\right).}
$$

This is the [stochastic exponential](../../../../../../doleans-dade-exponential.md) representation of a positive [continuous local martingale](../../../../../../continuous-local-martingale.md).

If $\langle X\rangle_\infty$ were finite on an event of positive probability, the [finite-bracket convergence lemma](../../../../../../finite-bracket-convergence-lemma.md) proved in Question 2(a) would make $X_t$ converge to a finite limit there. The exponential would then have a strictly positive limit, contradicting the assumed $M_t\to0$. Therefore

$$
\boxed{\langle X\rangle_\infty=\infty\quad\text{almost surely}.}
$$

This is the [divergent logarithmic clock for a positive local martingale tending to zero](../../../../../../divergent-logarithmic-clock-for-a-positive-local-martingale-tending-to-zero.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

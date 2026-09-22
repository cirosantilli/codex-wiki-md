<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Decompose $h=\Pi_1h+D^\dagger Dh$ using the [incidence pseudoinverse decomposition](../../../../../../incidence-pseudoinverse-decomposition.md). The [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) controls the constant component, and the duality of the $\ell_\infty$ and $\ell_1$ [norms](../../../../../../norm.md) controls the remaining component:

$$
\langle z,h\rangle\leq\|\Pi_1z\|_2\|h\|_2+\|(D^\dagger)^\top z\|_\infty\|Dh\|_1.
$$

On the stipulated event, the second term contributes at most $\lambda\|Dh\|_1$ after multiplication by $2/n$. The [triangle inequality](../../../../../../triangle-inequality.md) gives $\|Dh\|_1\leq\|D\widehat\theta\|_1+\|D\theta^*\|_1$, so the negative penalty in the [basic inequality for a penalized least-squares estimator](../../../../../../basic-inequality-for-a-penalized-least-squares-estimator.md) cancels. We obtain

$$
\boxed{\frac{\|h\|_2^2}{n}\leq2\lambda s(\theta^*)+\frac2n\|\Pi_1z\|_2\|h\|_2}
$$

on an event of [probability](../../../../../../probability.md) at least $1-\delta$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 210](../../../paper-210-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

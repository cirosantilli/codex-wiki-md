<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Work conditionally on a positive-probability atom of $\mathcal F_{T-1}$. Let $Z$ have the [conditional distribution](../../../../../../conditional-distribution.md) of $S_T$ there, and let $Z'$ be an independent copy of that conditional law. The finite sample space makes all [expectations](../../../../../../expected-value.md) finite. Then

$$
2\operatorname{Cov}(g(Z),Z)
=\mathbb E[(g(Z)-g(Z'))(Z-Z')].
$$

Strict increase of $g$ makes the integrand nonnegative, and strictly positive whenever $Z\ne Z'$. The [conditional variance](../../../../../../conditional-variance.md) is positive by part (c), so the [conditional distribution](../../../../../../conditional-distribution.md) is nondegenerate and $\mathbb P(Z\ne Z')>0$. Thus the numerator of the hedge ratio is strictly positive on every such atom. The denominator is also positive, giving

$$
\boxed{\pi_T>0\quad\text{almost surely}.}
$$

This is [strict positive covariance with an increasing payoff](../../../../../../strict-positive-covariance-with-an-increasing-payoff.md). The independent copy is taken from the [conditional distribution](../../../../../../conditional-distribution.md), not from an unrelated unconditional distribution.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

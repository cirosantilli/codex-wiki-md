<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Choose any strictly positive [pricing kernel](../../../../../../state-price-density.md) $Z\in\mathcal Z$. The assumed componentwise [expectations](../../../../../../expected-value.md) and the [linearity of expectation](../../../../../../linearity-of-expectation.md) give

$$
\mathbb E[Z(H\cdot P)]=H\cdot\mathbb E[ZP]=H\cdot p\leq0.
$$

The integrand is nonnegative, so its [expectation](../../../../../../expected-value.md) is also nonnegative and hence zero. A nonnegative [random variable](../../../../../../random-variable-split.md) with zero [expectation](../../../../../../expected-value.md) vanishes [almost surely](../../../../../../almost-sure-convergence.md). Since $Z>0$ [almost surely](../../../../../../almost-sure-convergence.md), this forces $H\cdot P=0$ [almost surely](../../../../../../almost-sure-convergence.md). **Both conclusions follow**:

$$
\boxed{H\cdot p=0,\qquad H\cdot P=0\quad\text{almost surely}.}
$$

The strict positivity of the [pricing kernel](../../../../../../state-price-density.md) is essential: a kernel allowed to vanish could miss a positive payoff on its zero set. No normalization $\mathbb EZ=1$ is assumed in this abstract market; that normalization follows only if a unit-priced unit-payoff cash asset is included.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 211](../../../paper-211-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

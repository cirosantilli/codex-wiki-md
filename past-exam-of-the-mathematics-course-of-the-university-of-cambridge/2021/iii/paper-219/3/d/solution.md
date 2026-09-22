<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $S=\sum_s(D_s-\bar D)^2$. Integrating out $M_0$ gives

$$
\boxed{
p(\tau^2\mid D)\propto
(\tau^2)^k(\tau^2+\sigma^2)^{-(N-1)/2}
\exp\left[-\frac{S}{2(\tau^2+\sigma^2)}\right]\mathbf1_{\{\tau^2\geq0\}}}.
$$

Near zero, integrability requires $k>-1$; at infinity it requires

$$
k-\frac{N-1}{2}<-1.
$$

For integer $k$ the posterior is proper exactly when

$$
\boxed{0\leq k<\frac{N-3}{2}}.
$$

The choice $k=0$ is allowed for $N>3$ and yields a proper posterior, but it is an improper flat prior on a scale parameter and is not invariant under reparameterization, so sensitivity to more principled scale priors should be checked.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 219](../../../paper-219-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

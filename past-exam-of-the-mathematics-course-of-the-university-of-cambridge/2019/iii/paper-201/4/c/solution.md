<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Fix a closed ball $\overline B(x,r)\subset D$ and let $\tau$ be its first exit time. By the [Strong Markov property](../../../../../../strong-markov-property.md), conditioning at $\tau$ gives

$$
\phi(x)=\mathbb E_x[\phi(X_\tau)].
$$

The [orthogonal invariance of Brownian motion](../../../../../../orthogonal-invariance-of-brownian-motion.md) implies that $X_\tau$ is uniformly distributed on the sphere $\partial B(x,r)$. Hence

$$
\phi(x)=\frac1{|\partial B(x,r)|}
\int_{\partial B(x,r)}\phi(y)\,dS(y).
$$

Thus $\phi$ has the [mean value property](../../../../../../mean-value-property-for-harmonic-functions.md) on every ball compactly contained in $D$. Since $0\leq\phi\leq1$, the mean-value characterization of [harmonic functions](../../../../../../harmonic-function.md) yields

$$
\boxed{\Delta\phi=0\quad\text{in }D.}
$$

This function is the [harmonic measure](../../../../../../harmonic-measure.md) of $A$ viewed from $x$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

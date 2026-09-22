<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [strong law of large numbers](../../../../../../strong-law-of-large-numbers.md) gives

$$
\frac{S_n}{n}\longrightarrow\mathbb E[X_1]=2p-1>0
\qquad\text{almost surely}.
$$

Because $0<\lambda<1$, it follows that $\lambda^{S_n}\to0$ almost surely. If this martingale were [uniformly integrable](../../../../../../uniform-integrability.md), almost-sure convergence would imply convergence in $L^1$, and therefore

$$
\mathbb E[\lambda^{S_n}]\longrightarrow0.
$$

But the martingale has constant expectation $\mathbb E[\lambda^{S_n}]=1$. This contradiction proves that

$$
\boxed{(\phi(S_n))_{n\geq0}\text{ is not uniformly integrable}.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $\sigma$ be the first time Brownian motion started outside the unit half-disc reaches its semicircular boundary. A path that reaches $A$ must first cross that semicircle. The [Strong Markov property](../../../../../../strong-markov-property.md) at $\sigma$ gives

$$
\mathbb E_z[\operatorname{Im}B_\tau]
=\int_0^\pi p(z,e^{i\theta})
\mathbb E_{e^{i\theta}}[\operatorname{Im}B_\tau]\,d\theta.
$$

Take $z=iy$, multiply by $y$, and let $y\to\infty$. The [Brownian representation of half-plane capacity](../../../../../../brownian-representation-of-half-plane-capacity.md) identifies the left side with $\operatorname{hcap}(A)$, while part b gives

$$
yp(iy,e^{i\theta})\longrightarrow\frac2\pi\sin\theta.
$$

Since the exit height is between zero and one, the [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) applies and yields

$$
\boxed{\operatorname{hcap}(A)
=\frac2\pi\int_0^\pi
\mathbb E_{e^{i\theta}}[\operatorname{Im}B_\tau]
\sin\theta\,d\theta.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 203](../../../paper-203-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

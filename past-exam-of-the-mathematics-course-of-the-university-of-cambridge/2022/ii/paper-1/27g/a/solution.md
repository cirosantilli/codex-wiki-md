<h1 id="27g/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $(X_n)$ be [independent random variables](../../../../../../independent-random-variables.md) and let

$$
\mathcal T=\bigcap_{n\geq1}\sigma(X_n,X_{n+1},\ldots)
$$

be their [tail sigma-algebra](../../../../../../tail-sigma-algebra.md). The [Kolmogorov zero-one law](../../../../../../kolmogorov-s-zero-one-law.md) states that every $A\in\mathcal T$ has probability zero or one.

Indeed, $A$ is independent of $\sigma(X_1,\ldots,X_n)$ for every $n$. The union of these finite-coordinate sigma-algebras generates $\sigma(X_1,X_2,\ldots)$, and [independence extended from generating pi-systems](../../../../../../independence-extended-from-generating-pi-systems.md) shows that $A$ is independent of that entire sigma-algebra. Since $A$ itself belongs to it,

$$
\mathbb P(A)=\mathbb P(A\cap A)=\mathbb P(A)^2,
$$

so $\mathbb P(A)\in\{0,1\}$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [27G](../../27g.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

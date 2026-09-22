<h1 id="27g/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

On a probability space carrying an infinite [IID](../../../../../../independent-and-identically-distributed-random-variables.md) sequence $(X_n)$ with law $m$, map $\omega$ to $(X_1(\omega),X_2(\omega),\ldots)$. Its pushforward measure $\mu$ satisfies

$$
\mu\!\left(\prod_{n\geq1}A_n\right)=\prod_{n\geq1}m(A_n)
$$

for every cylinder set. Cylinder sets form a [pi-system](../../../../../../pi-system.md) generating $\sigma(\mathcal C)$, so the [sigma-finite uniqueness theorem for measures](../../../../../../sigma-finite-uniqueness-theorem-for-measures.md) proves uniqueness. This is the countable [product measure](../../../../../../product-measure.md) $m^{\otimes\mathbb N}$.

For a cylinder $A=A_1\times\cdots\times A_N\times\mathbb R\times\cdots$,

$$
\mu(\theta^{-1}A)=m(\mathbb R)m(A_1)\cdots m(A_N)=\mu(A).
$$

The same generating-class argument extends this equality to every measurable set, so $\theta$ is a [measure-preserving transformation](../../../../../../measure-preserving-transformation.md).

If $A=\theta^{-1}A$, then $A=\theta^{-n}A$ for every $n$, so membership in $A$ is independent of the first $n$ coordinates. Thus $A$ belongs to the tail sigma-algebra. The zero-one law gives $\mu(A)\in\{0,1\}$, proving that the shift is [ergodic](../../../../../../ergodicity.md).

## ↑ Ancestors (11)

1. [B](../b.md)
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

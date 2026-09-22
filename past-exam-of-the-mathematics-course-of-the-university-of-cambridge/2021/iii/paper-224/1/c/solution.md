<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Fix $\delta>0$ and choose

$$
\tau_n=\exp\{n(D(P\Vert Q)-\delta)\}.
$$

Under $P$, the [weak law of large numbers](../../../../../../weak-law-of-large-numbers.md) makes the normalized log likelihood ratio converge in probability to $D(P\Vert Q)$, so $P^{\otimes n}(B_n(\tau_n))\to1$. On this [Neyman-Pearson decision region](../../../../../../neyman-pearson-decision-region.md),

$$
Q^{\otimes n}\leq\tau_n^{-1}P^{\otimes n},
$$

and hence

$$
\beta_n\leq e^{-n(D(P\Vert Q)-\delta)}.
$$

Letting $\delta\downarrow0$ proves the direct bound.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 224](../../../paper-224-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

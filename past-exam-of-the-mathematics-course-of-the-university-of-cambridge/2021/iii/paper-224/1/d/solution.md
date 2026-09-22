<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For any region $B_n$ with $P^{\otimes n}(B_n)\geq1-\varepsilon$, let

$$
C_n=\left\{x_1^n:n^{-1}\log\frac{P^{\otimes n}(x_1^n)}{Q^{\otimes n}(x_1^n)}
\leq D(P\Vert Q)+\delta\right\}.
$$

The [weak law of large numbers](../../../../../../weak-law-of-large-numbers.md) gives $P^{\otimes n}(C_n)\to1$, so $P^{\otimes n}(B_n\cap C_n)\geq1-\varepsilon-o(1)$. Therefore

$$
\beta_n\geq Q^{\otimes n}(B_n\cap C_n)
\geq e^{-n(D(P\Vert Q)+\delta)}\{1-\varepsilon-o(1)\}.
$$

**Thus $\limsup-n^{-1}\log\beta_n\leq D(P\Vert Q)+\delta$; let $\delta\downarrow0$.**

## ↑ Ancestors (11)

1. [D](../d.md)
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

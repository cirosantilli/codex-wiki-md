<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $B_n$ be the region on which the test chooses $P_n$. Then

$$
e_1^{(n)}(B_n)+e_2^{(n)}(B_n)
=P_n(B_n^c)+Q_n(B_n)
=1-\{P_n(B_n)-Q_n(B_n)\}.
$$

Minimizing over decision regions is therefore equivalent to maximizing the signed difference. Part b gives

$$
\min_{B_n\subseteq A^n}P_e^{(n)}(B_n)
=1-\sup_{B_n}\{P_n(B_n)-Q_n(B_n)\}
=1-\frac12\lVert P_n-Q_n\rVert_{\rm TV}.
$$

The minimizing region is $\{x:P_n(x)\geq Q_n(x)\}$, the equal-prior [Neyman-Pearson decision region](../../../../../../neyman-pearson-decision-region.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 224](../../../paper-224-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

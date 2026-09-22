<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Writing $P,Q$ for the laws of $X,Y$, respectively, and using [Jensen inequality](../../../../../../jensen-s-inequality.md) for the concave [natural logarithm](../../../../../../natural-logarithm.md),

$$
\begin{aligned}
\mathbb E_Pg-D_e(P\Vert Q)
&=\sum_xP(x)\log_e\frac{e^{g(x)}Q(x)}{P(x)}\\
&\leq\log_e\sum_xP(x)\frac{e^{g(x)}Q(x)}{P(x)}\\
&=\log_e\mathbb E_Qe^{g(Y)}.
\end{aligned}
$$

This is the lower-bound half of the [Gibbs variational principle for relative entropy](../../../../../../gibbs-variational-principle-for-relative-entropy.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 224](../../../paper-224-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

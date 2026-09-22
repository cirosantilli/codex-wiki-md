<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The elementary [logarithm inequality](../../../../../../logarithm-inequality.md) $\log_2u\leq(\log_2e)(u-1)$ gives

$$
D(P\Vert Q)
\leq(\log e)\sum_xP(x)\left(\frac{P(x)}{Q(x)}-1\right).
$$

Since $\sum_x(P(x)-Q(x))=0$,

$$
\sum_xP(x)\frac{P(x)-Q(x)}{Q(x)}
=\sum_x\frac{(P(x)-Q(x))^2}{Q(x)}
=\chi^2(P\Vert Q).
$$

This proves $D(P\Vert Q)\leq(\log e)\chi^2(P\Vert Q)$, relating [relative entropy](../../../../../../kullback-leibler-divergence.md) to [chi-squared divergence](../../../../../../chi-squared-divergence.md).

## ↑ Ancestors (11)

1. [C](../c.md)
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

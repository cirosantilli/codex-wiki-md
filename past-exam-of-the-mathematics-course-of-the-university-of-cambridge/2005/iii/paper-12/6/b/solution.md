<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The first right endpoint is the smallest of $n$ [independent](../../../../../../independent-random-variables.md) pair maxima. A maximum exceeds $r$ with [probability](../../../../../../probability.md) $1-r^2$, so for $0\le x\le\sqrt n$,

$$
\Pr(R_1\ge x/\sqrt n)=\left(1-\frac{x^2}{n}\right)^n.
$$

Taking the limit gives the requested, correctly normalized result

$$
\boxed{\Pr(\sqrt nR_1\ge x)\longrightarrow e^{-x^2}\quad(x>0).}
$$

Thus $\sqrt nR_1$ converges to a continuous nonnegative limit $W$ with survival function $\Pr(W\ge x)=e^{-x^2}$. In particular the scaled first right endpoint is tight. This calculation uses maxima of pairs, not the first [order statistic](../../../../../../order-statistic.md) of all $2n$ individual endpoints, which would have a different scale. The converted TeX loses the formula in this part; the displayed limit has been recovered directly from the PDF.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 12](../../../paper-12-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

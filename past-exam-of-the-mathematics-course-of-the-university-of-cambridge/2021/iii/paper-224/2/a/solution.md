<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For finite $m$, independence and conditional [subadditivity of information entropy](../../../../../../subadditivity-of-information-entropy.md) give

$$
\begin{aligned}
\sum_{i=1}^mI(X_i;Z)
&=H(X_1^m)-\sum_iH(X_i\mid Z)\\
&\leq H(X_1^m)-H(X_1^m\mid Z)
=I(X_1^m;Z)\leq H(Z).
\end{aligned}
$$

The partial sums increase because [mutual information](../../../../../../mutual-information.md) is nonnegative. Taking $m\to\infty$ proves $H(Z)\geq\sum_{i\geq1}I(X_i;Z)$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 224](../../../paper-224-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

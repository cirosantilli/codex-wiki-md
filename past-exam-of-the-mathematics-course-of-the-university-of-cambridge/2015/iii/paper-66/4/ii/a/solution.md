<h1 id="4/ii/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $Y_i=-\log_2P_Z(Z_i)$. Since the alphabet is finite, these [independent and identically distributed random variables](../../../../../../../independent-and-identically-distributed-random-variables.md) are finite almost surely, have mean $H(Z)$, and have finite variance $v$. Also

$$
-\frac1n\log_2P_Z^n(Z^{(n)})=\frac1n\sum_{i=1}^nY_i.
$$

The [weak law of large numbers](../../../../../../../weak-law-of-large-numbers.md) says that this average converges in probability to $H(Z)$. Thus

$$
\boxed{\lim_{n\to\infty}\Pr\bigl(Z^{(n)}\in T_\delta^n(P_Z)\bigr)=1\quad(\delta>0).}
$$

One can also state the quantitative [Chebyshev inequality](../../../../../../../chebyshev-inequality.md) bound $\Pr(Z^{(n)}\notin T_\delta^n)\leq v/(n\delta^2)$. If $v=0$, every word of positive probability is in the [typical set](../../../../../../../typical-set.md). This is the finite-alphabet [asymptotic equipartition property](../../../../../../../asymptotic-equipartition-property.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [Ii](../../ii.md)
3. [4](../../../4.md)
4. [Paper 66](../../../../paper-66-split.md)
5. [Iii](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)

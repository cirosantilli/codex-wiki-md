<h1 id="27i/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The unrestricted categorical MLE is $\widetilde\pi_j=N_j/n$, so the multinomial combinatorial factor cancels from the likelihood ratio and

$$
W_n=2\sum_jN_j\log\frac{N_j}{n\widehat\pi_j}.
$$

Assume the true cell probabilities are positive and the null has identifiable dimension $d$ with full-rank information. With [probability](../../../../../../probability.md) tending to one, all $N_j$ are positive. Put $\delta_j=n\widehat\pi_j-N_j$. Regular estimation gives $\delta_j=O_p(\sqrt n)$ and $N_j$ of order $n$. Expanding $-2N_j\log(1+\delta_j/N_j)$ yields

$$
W_n=\sum_j\left[-2\delta_j+\frac{\delta_j^2}{N_j}+O_p(n^{-1/2})\right].
$$

The linear terms cancel exactly because $\sum_j\delta_j=0$. Therefore

$$
\boxed{W_n=\sum_{j=1}^K\frac{(N_j-n\widehat\pi_j)^2}{N_j}+o_p(1)
\ \Rightarrow\ \chi^2_{K-1-d}.}
$$

The full [probability](../../../../../../probability.md) simplex has dimension $K-1$, explaining the degrees of freedom. Existence and uniqueness of an MLE alone do not supply all Wilks regularity assumptions; positivity, smoothness and the local rank condition are also needed. The displayed approximation is not a finite-sample prescription for division by a zero observed count.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [27I](../../27i.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

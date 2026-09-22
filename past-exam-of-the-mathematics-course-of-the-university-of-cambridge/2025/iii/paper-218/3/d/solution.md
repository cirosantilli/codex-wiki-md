<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The limiting conditional error of one-nearest-neighbour classification is $1-\sum_kp_k(x)^2$. Put $M=\max_kp_k(x)$ and $r=1-M$. By the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md), the other $K-1$ probabilities satisfy

$$
\sum_{k:p_k\ne M}p_k^2\geq\frac{r^2}{K-1}.
$$

Consequently

$$
1-\sum_kp_k^2
\leq1-(1-r)^2-\frac{r^2}{K-1}
=2r-\frac K{K-1}r^2.
$$

Now $\mathbb Er=R_{\mathrm{Bayes}}$, and [Jensen inequality](../../../../../../jensen-s-inequality.md) gives $\mathbb Er^2\geq(\mathbb Er)^2$. Taking expectations proves

$$
\boxed{\lim_{n\to\infty}R(h_n^{\mathrm{1NN}})
\leq2R_{\mathrm{Bayes}}-\frac K{K-1}R_{\mathrm{Bayes}}^2.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

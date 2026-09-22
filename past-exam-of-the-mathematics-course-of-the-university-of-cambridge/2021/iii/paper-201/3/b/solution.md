<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The increment variance is

$$
\operatorname{Var}(\xi_k)=1-(2p-1)^2=4p(1-p),
$$

so independence gives

$$
\operatorname{Var}(S_n)=4np(1-p).
$$

Linear interpolation makes the supremum of the absolute centered process occur at an integer time. The [Doob L2 maximal inequality](../../../../../../doob-l2-maximal-inequality.md) therefore gives

$$
\begin{aligned}
\mathbb E\sup_{0\leq t\leq1}|S_t^{(n)}-\mu t|^2
&=\frac1{n^2}\mathbb E\max_{0\leq k\leq n}|M_k|^2\\
&\leq\frac4{n^2}\mathbb E M_n^2
=\frac{16p(1-p)}n
\leq\boxed{\frac4n}.
\end{aligned}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

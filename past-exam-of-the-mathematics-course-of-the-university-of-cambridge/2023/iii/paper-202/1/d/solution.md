<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Set $g_\epsilon(x)=x/\sqrt{\epsilon^2+x^2}$ and $g(x)=\operatorname{sgn}(x)$, with $g(0)=0$. For every $s>0$, the [normal distribution](../../../../../../normal-distribution.md) of $B_s$ has no atom at zero, so $g_\epsilon(B_s)\to g(B_s)$ almost surely. Since $|g_\epsilon-g|\leq2$, the [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) and [Tonelli theorem](../../../../../../tonelli-theorem.md) give

$$
\mathbb E\int_0^T|g_\epsilon(B_s)-g(B_s)|^2ds\longrightarrow0.
$$

The [Itô isometry](../../../../../../ito-isometry.md) followed by the [Doob L2 maximal inequality](../../../../../../doob-l2-maximal-inequality.md) now yields

$$
\mathbb E\sup_{t\leq T}\left|
\int_0^t\bigl(g_\epsilon(B_s)-g(B_s)\bigr)dB_s
\right|^2
\leq4\mathbb E\int_0^T|g_\epsilon(B_s)-g(B_s)|^2ds\longrightarrow0.
$$

**Thus the stochastic integrals converge ucp to $\int_0^t\operatorname{sgn}(B_s)dB_s$.**

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

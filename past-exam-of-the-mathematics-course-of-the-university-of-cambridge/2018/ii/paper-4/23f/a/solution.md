<h1 id="23f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Set

$$
g=he^{-\Phi/2},
\qquad
V=\frac{|\Phi'|^2}{4}-\frac{\Phi''}{2}.
$$

The [ground-state transform for a weighted Dirichlet energy](../../../../../../ground-state-transform-for-a-weighted-dirichlet-energy.md), obtained by expanding the square and using [integration by parts](../../../../../../integration-by-parts.md), is

$$
\begin{aligned}
\int_{\mathbb R}|h'|^2e^{-\Phi}
&=\int_{\mathbb R}\left|g'+\frac{\Phi'}2g\right|^2\\
&=\int_{\mathbb R}|g'|^2+\int_{\mathbb R}V|g|^2.
\end{aligned}
$$

The boundary term vanishes because $h$, and hence $g$, has [compact support](../../../../../../compact-support.md).

Since $V(x)\to\ell>0$, choose $R_0$ so that $V\geq\ell/2$ when $|x|\geq R_0$, and set

$$
\lambda_1=\frac\ell2,
\qquad
K_1=\max\left\{0,-\min_{|x|\leq R_0}V(x)\right\}.
$$

For every $R\geq R_0$, discard the nonnegative $|g'|^2$ term and the nonnegative contribution from $R_0\leq|x|\leq R$ to obtain

$$
\int_{\mathbb R}|h'|^2e^{-\Phi}
\geq\lambda_1\int_{|x|\geq R}|g|^2-K_1\int_{|x|\leq R}|g|^2.
$$

Because $|g|^2=|h|^2e^{-\Phi}$, this is exactly the required estimate.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [23F](../../23f.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

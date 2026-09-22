<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Applying the regression operator from part i gives

$$
\mathbb E[Y(t)\mid X]
=\sum_{k=1}^\infty a_k
\left\{\sum_{l=1}^\infty
\frac{\mathbb E[a_kb_l]}{\lambda_k}u_l(t)\right\}.
$$

The uncorrelated scores satisfy $\operatorname{Var}(a_k)=\lambda_k$, while $\operatorname{Var}(Y(t))=\sum_l\gamma_lu_l(t)^2$. Hence

$$
\boxed{
R(t)=
\frac{\displaystyle
\sum_{k=1}^\infty\frac1{\lambda_k}
\left(\sum_{l=1}^\infty\mathbb E[a_kb_l]u_l(t)\right)^2}
{\displaystyle\sum_{l=1}^\infty\gamma_lu_l(t)^2}}.
$$

The sign cancellations from part ii leave every squared numerator term unchanged; changing the sign of $u_l$ also leaves each denominator term unchanged. Thus $R(t)$ is sign invariant.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 225](../../../paper-225-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

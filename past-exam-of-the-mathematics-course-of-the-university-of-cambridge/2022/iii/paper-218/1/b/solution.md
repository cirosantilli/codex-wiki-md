<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $x_i^T$ be row $i$ of the design matrix, $\eta_i=x_i^T\beta=1/\mu_i$, and $\gamma=1/\phi$. The full [log-likelihood](../../../../../../log-likelihood.md) is

$$
\ell(\beta,\gamma)
=\sum_{i=1}^{61}
\left\{
\gamma\log\gamma+\gamma\log\eta_i-\log\Gamma(\gamma)
+(\gamma-1)\log y_i-\gamma y_i\eta_i
\right\}.
$$

Differentiation gives the [score function](../../../../../../informant-function.md)

$$
\nabla_\beta\ell
=\gamma X^T(\mu-Y),
\qquad
\mu_i=\eta_i^{-1},
$$

and

$$
-\nabla_\beta^2\ell
=\gamma X^T\operatorname{diag}(\mu_i^2)X.
$$

The Hessian does not depend on $Y$, so the [Fisher information matrix](../../../../../../fisher-information-matrix.md) is

$$
\boxed{\mathcal I_\beta
=\frac1\phi X^TWX,
\qquad
W=\operatorname{diag}(\mu_i^2).}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Expanding the [ordinary least squares](../../../../../../ordinary-least-squares.md) objective gives

$$
Q(\beta)=Y^TY-2\beta^TX^TY+\beta^TX^TX\beta,
\qquad \nabla Q=2X^T(X\beta-Y),\quad \nabla^2Q=2X^TX.
$$

For a nonzero vector $v$, $v^TX^TXv=\|Xv\|^2>0$, since the [design matrix](../../../../../../design-matrix.md) has [matrix rank](../../../../../../matrix-rank.md) $p$. The [Hessian matrix](../../../../../../hessian-matrix.md) is therefore [positive-definite](../../../../../../positive-definite-bilinear-form.md), and $Q$ is strictly [convex](../../../../../../convex-function.md). Solving its [normal equations](../../../../../../normal-equation.md) gives the unique [least-squares estimator](../../../../../../ordinary-least-squares-estimators.md):

$$
\boxed{\widehat\beta=(X^TX)^{-1}X^TY.}
$$

Indeed, expansion about this stationary point and $X^T(Y-X\widehat\beta)=0$ give $Q(\beta)=Q(\widehat\beta)+(\beta-\widehat\beta)^TX^TX(\beta-\widehat\beta)$, which also proves the global minimum directly.

Define the [hat matrix](../../../../../../hat-matrix.md) $H=X(X^TX)^{-1}X^T$. It is a [symmetric matrix](../../../../../../symmetric-matrix.md) and an [idempotent linear map](../../../../../../projection-linear-algebra.md), since $H^T=H$ and $H^2=H$, and its image is the column space of $X$. Thus $H$ is the [orthogonal projection](../../../../../../orthogonal-projection.md) onto the fitted mean space. The [fitted values](../../../../../../fitted-values.md) are $HY$ and the [regression residual](../../../../../../regression-residual.md) vector is $(I-H)Y$. Because $I-H$ is also a [symmetric matrix](../../../../../../symmetric-matrix.md) and an [idempotent linear map](../../../../../../projection-linear-algebra.md),

$$
\boxed{Q(\widehat\beta)=Y^T(I-H)^T(I-H)Y=Y^T(I-H)Y.}
$$

These minimization and projection identities do not need errors with a [normal distribution](../../../../../../normal-distribution.md); the [normal linear model](../../../../../../normal-linear-model.md) becomes relevant to the distributional calculations.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 41](../../../paper-41-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

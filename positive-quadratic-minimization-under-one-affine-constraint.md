# Positive quadratic minimization under one affine constraint

↑ **Parent:** [Positive-definite quadratic optimization](positive-definite-quadratic-optimization.md)

Let $H$ be a symmetric [positive-definite matrix](positive-definite-matrix.md), $a\ne0$, and $b\in\mathbb R$. Then

$$
z_* =\frac{bH^{-1}a}{a^TH^{-1}a}
$$

is the unique solution of minimizing the [quadratic form](quadratic-form-split.md) $z^THz$ under the affine [optimization constraint](optimization-constraint.md) $a^Tz=b$. The minimum value is $b^2/(a^TH^{-1}a)$.

The denominator is positive because $H^{-1}$ is a [positive-definite matrix](positive-definite-matrix.md). The [Lagrange multiplier](lagrange-multiplier.md) equations $2Hz=\lambda a$ give the displayed candidate and verify the constraint. For a global proof, any feasible perturbation $u=z-z_*$ satisfies $a^Tu=0$. Hence

$$
z^THz-z_*^THz_*=2z_*^THu+u^THu=u^THu.
$$

This is positive for every nonzero $u$. The result also handles several independent quadratic blocks by taking $H$ to be their [block diagonal matrix](block-diagonal-matrix.md) and concatenating their variables.

## ↑ Ancestors (5)

1. [Positive-definite quadratic optimization](positive-definite-quadratic-optimization.md)
2. [Mathematical optimization](mathematical-optimization-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2021/discrete-mathematics-continuous-mathematics-and-probability/5/d/solution.md)

<h1 id="2/vi/solution">Solution</h1>

↑ **Parent:** [Vi](../vi.md)

The relevant nonlinear [generalized singular vector](../../../../../../generalized-singular-vector.md) relation, without imposing unit-data normalization, is

$$
p=\lambda K^*Ku^\dagger\in\partial J(u^\dagger),\qquad u^\dagger\ne0.
$$

This is a [generalized eigenfunction in the forward-operator metric](../../../../../../generalized-eigenfunction-in-the-forward-operator-metric.md), rather than a distributional generalized eigenfunction of a linear operator. It supplies the [normal-operator source condition](../../../../../../normal-operator-source-condition.md) with $v=\lambda u^\dagger$. For a [convex positively one-homogeneous functional](../../../../../../convex-positively-one-homogeneous-functional.md), the [subgradient inequality](../../../../../../subgradient-inequality.md) applied at zero and at $2u^\dagger$ gives $\langle p,u^\dagger\rangle=J(u^\dagger)$. If $Ku^\dagger\ne0$, then

$$
\lambda=\frac{J(u^\dagger)}{\|Ku^\dagger\|^2}.
$$

Assume the usual positive eigenvalue $\lambda>0$ and $0<\alpha\lambda\leq1$. By [positive homogeneity](../../../../../../positively-homogeneous-function-degree-one.md),

$$
D_J^p((1-\alpha\lambda)u^\dagger,u^\dagger)=0.
$$

The [shifted-comparator Bregman bound](../../../../../../shifted-comparator-bregman-bound.md) therefore yields

$$
\boxed{D_J^p(u_\alpha,u^\dagger)=0,\qquad Ku_\alpha=(1-\alpha\lambda)Ku^\dagger.}
$$

The vector $(1-\alpha\lambda)u^\dagger$ is itself a minimizer: $p$ remains a [subgradient](../../../../../../subgradient.md) along the nonnegative ray, and substitution satisfies the [subgradient optimality condition](../../../../../../subgradient-optimality-condition.md). If $K$ is injective, this also proves $u_\alpha=(1-\alpha\lambda)u^\dagger$. Otherwise distinct minimizers can differ in the [kernel](../../../../../../kernel-of-a-linear-map.md) while sharing the same predicted data.

For a nonnegative [convex positively one-homogeneous functional](../../../../../../convex-positively-one-homogeneous-functional.md), the branch continues as $(1-\alpha\lambda)_+u^\dagger$ above the threshold, since $p/(\alpha\lambda)\in\partial J(0)$ there. Nonnegativity is needed for that clipping argument; bare positive homogeneity allows signed linear functionals.

**Zero Bregman distance does not imply exact recovery.** For $K=I$, $J(s)=|s|$, $u^\dagger=a>0$ and $0<\alpha<a$, the minimizer is $u_\alpha=a-\alpha\ne a$, but $D_J^1(a-\alpha,a)=0$. Both points touch the same supporting line, as described by [zero Bregman distance and supporting faces](../../../../../../zero-bregman-distance-and-supporting-faces.md).

## ↑ Ancestors (11)

1. [Vi](../vi.md)
2. [2](../../2.md)
3. [Paper 326](../../../paper-326-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

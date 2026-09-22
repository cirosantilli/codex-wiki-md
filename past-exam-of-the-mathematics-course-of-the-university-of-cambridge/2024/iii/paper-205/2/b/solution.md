<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The differential of the [log-determinant](../../../../../../log-determinant.md) is $d\log\det\Omega=\operatorname{Tr}(\Omega^{-1}d\Omega)$. The [subdifferential](../../../../../../subdifferential.md) of the entrywise $\ell^1$ norm consists of symmetric matrices $Z$ with

$$
Z_{ij}=\operatorname{sgn}(\Omega_{ij})\quad\hbox{if }\Omega_{ij}\ne0,
\qquad Z_{ij}\in[-1,1]\quad\hbox{if }\Omega_{ij}=0.
$$

The [Karush-Kuhn-Tucker conditions](../../../../../../karush-kuhn-tucker-conditions.md) for the [Graphical Lasso](../../../../../../graphical-lasso.md) are therefore

$$
-\widehat\Omega^{-1}+S+\lambda Z=0,
\qquad Z\in\partial\lVert\widehat\Omega\rVert_{1,\mathrm{entry}}.
$$

Because $-\log\det\Omega$ is [strictly convex](../../../../../../strictly-convex-function.md) on the [positive-definite matrices](../../../../../../positive-definite-matrix.md), these conditions characterize the unique minimizer whenever it exists.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 205](../../../paper-205-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

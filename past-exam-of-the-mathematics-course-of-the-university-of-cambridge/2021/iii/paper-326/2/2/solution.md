<h1 id="2/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A $J$-minimizing solution is an exact solution $u_J^\dagger$ satisfying

$$
Au_J^\dagger=f,
\qquad
J(u_J^\dagger)=\inf\{J(u):Au=f\}.
$$

The [source condition in variational regularization](../../../../../../source-condition-in-variational-regularization.md) says that some $p^\dagger\in Y$ satisfies

$$
\boxed{A^*p^\dagger\in\partial J(u_J^\dagger)},
$$

where $\partial J$ is the [subdifferential](../../../../../../subdifferential.md).

Fix $\alpha>0$. The [subgradient optimality condition](../../../../../../subgradient-optimality-condition.md) for

$$
F_g(u)=\frac12\|Au-g\|_Y^2+\alpha J(u)
$$

at $u_J^\dagger$ is

$$
0\in A^*(Au_J^\dagger-g)+\alpha\partial J(u_J^\dagger).
$$

If the source condition holds, choose $g=f+\alpha p^\dagger$. Since $Au_J^\dagger=f$, the displayed inclusion holds. Because the objective is a [convex function](../../../../../../convex-function.md), this condition is necessary and sufficient for global minimality.

Conversely, if the stated range condition holds for some $g$, optimality supplies $\xi\in\partial J(u_J^\dagger)$ with

$$
A^*(f-g)+\alpha\xi=0.
$$

**Thus $\xi=A^*((g-f)/\alpha)$, which is precisely the source condition. This proves the equivalence.**

## ↑ Ancestors (11)

1. [2](../2.md)
2. [2](../../2.md)
3. [Paper 326](../../../paper-326-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $\widehat u_\alpha$ minimize the nonsquared-residual objective. Comparison with $u^\dagger$ gives

$$
\|A\widehat u_\alpha-f\|_Y
+\alpha[J(\widehat u_\alpha)-J(u^\dagger)]\leq0.
$$

The source subgradient inequality gives

$$
J(\widehat u_\alpha)-J(u^\dagger)
\geq\langle w^\dagger,A\widehat u_\alpha-f\rangle.
$$

Consequently,

$$
0\geq
\|A\widehat u_\alpha-f\|_Y
+\alpha\langle w^\dagger,A\widehat u_\alpha-f\rangle
\geq
(1-\alpha\|w^\dagger\|_{Y^*})
\|A\widehat u_\alpha-f\|_Y.
$$

Thus for

$$
\boxed{\alpha_0=
\begin{cases}
\|w^\dagger\|_{Y^*}^{-1},&w^\dagger\ne0,\\
+\infty,&w^\dagger=0,
\end{cases}}
$$

every $0<\alpha<\alpha_0$ forces $A\widehat u_\alpha=f$. The original comparison then gives $J(\widehat u_\alpha)\leq J(u^\dagger)$, so $\widehat u_\alpha$ is itself $J$-minimizing. If $J$ is [strictly convex](../../../../../../strictly-convex-function.md), its restriction to the affine solution set has at most one minimizer, hence $\widehat u_\alpha=u^\dagger$. This is an [exact penalty method](../../../../../../exact-penalty-method.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 326](../../../paper-326-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

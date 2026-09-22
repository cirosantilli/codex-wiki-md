<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Euclidean projection onto a convex set](../../../../../../euclidean-projection-onto-a-convex-set.md) is nonexpansive, and $x^*=P_C(x^*)$ because the optimum is feasible. Therefore the [projected subgradient method](../../../../../../projected-subgradient-method.md) satisfies

$$
\begin{aligned}
\lVert x_{i+1}-x^*\rVert_2^2
&\leq\lVert x_i-tg_i-x^*\rVert_2^2\\
&=\lVert x_i-x^*\rVert_2^2
-2t\langle g_i,x_i-x^*\rangle+t^2\lVert g_i\rVert_2^2.
\end{aligned}
$$

The [subgradient inequality](../../../../../../subgradient-inequality.md) gives $\langle g_i,x_i-x^*\rangle\geq f(x_i)-f^*$, while [Lipschitz continuity](../../../../../../lipschitz-continuity.md) of the finite [convex function](../../../../../../convex-function.md) gives $\lVert g_i\rVert_2\leq G$. Hence

$$
2t\bigl(f(x_i)-f^*\bigr)
\leq \lVert x_i-x^*\rVert_2^2-
\lVert x_{i+1}-x^*\rVert_2^2+t^2G^2.
$$

Summing this telescoping inequality for $0\leq i<k$, and then bounding the smallest term by the average, yields

$$
\min_{0\leq i<k}f(x_i)-f^*
\leq\frac{\lVert x_0-x^*\rVert_2^2}{2tk}
+\frac{tG^2}{2}.
$$

Writing $D=\lVert x_0-x^*\rVert_2$, the right-hand side is minimized by the constant [step size](../../../../../../step-size.md)

$$
t=\frac{D}{G\sqrt{k}}.
$$

Substitution gives

$$
\boxed{\min_{0\leq i<k}f(x_i)-f^*\leq\frac{GD}{\sqrt{k}}}.
$$

If $D=0$, the initial point is already optimal and the result is immediate.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 339](../../../paper-339-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

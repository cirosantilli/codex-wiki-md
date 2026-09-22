<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The function $\phi(x)=\max_{v\in C}\langle x,v\rangle$ is the [support function](../../../../../../support-function.md) $\sigma_C$. For a nonempty compact [convex set](../../../../../../convex-set.md),

$$
\sigma_C^*(v)=
\begin{cases}
0,&v\in C,\\
+\infty,&v\notin C,
\end{cases}
$$

so its [convex conjugate](../../../../../../convex-conjugate.md) is the [indicator function](../../../../../../indicator-function.md) $\iota_C$. Applying the [Moreau decomposition](../../../../../../moreau-decomposition.md),

$$
\operatorname{prox}_{t\phi}(y)
=y-t\operatorname{prox}_{t^{-1}\iota_C}(y/t).
$$

Multiplication of an [indicator function](../../../../../../indicator-function.md) by a positive scalar does not change it, and its [proximal operator](../../../../../../proximal-operator.md) is the [Euclidean projection onto a convex set](../../../../../../euclidean-projection-onto-a-convex-set.md). Therefore

$$
\boxed{\operatorname{prox}_{t\phi}(y)=y-tP_C(y/t)}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 339](../../../paper-339-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

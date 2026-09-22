<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a proper lower-semicontinuous [convex function](../../../../../../convex-function.md) $f$, its [proximal operator](../../../../../../proximal-operator.md) is

$$
\operatorname{prox}_f(y)=
\arg\min_x\left\{f(x)+\frac12\lVert x-y\rVert_2^2\right\}.
$$

The squared norm is strongly convex, so the minimizer is unique. The [subdifferential sum rule](../../../../../../subdifferential-sum-rule.md) gives the necessary and sufficient condition

$$
x=\operatorname{prox}_f(y)
\quad\Longleftrightarrow\quad
0\in\partial f(x)+x-y
\quad\Longleftrightarrow\quad
y-x\in\partial f(x).
$$

More generally,

$$
x=\operatorname{prox}_{tf}(y)
\quad\Longleftrightarrow\quad
u:=\frac{y-x}{t}\in\partial f(x).
$$

The subgradient inversion rule for the [convex conjugate](../../../../../../convex-conjugate.md) says $u\in\partial f(x)$ exactly when $x\in\partial f^*(u)$. Hence

$$
\frac yt-u=\frac xt\in\frac1t\partial f^*(u)
=\partial(t^{-1}f^*)(u),
$$

which is precisely the proximal optimality condition

$$
u=\operatorname{prox}_{t^{-1}f^*}(y/t).
$$

Since $x=y-tu$, this proves the generalized [Moreau decomposition](../../../../../../moreau-decomposition.md)

$$
\boxed{\operatorname{prox}_{tf}(y)=
y-t\operatorname{prox}_{t^{-1}f^*}(y/t)}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
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

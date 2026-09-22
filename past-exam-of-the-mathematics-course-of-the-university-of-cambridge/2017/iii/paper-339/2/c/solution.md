<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write a test [vector](../../../../../../vector.md) as $(u,v)$ and put $s=\sum_i u_i$, $t=\sum_jv_j$. Its [quadratic form](../../../../../../quadratic-form.md) against the block-constant [matrix](../../../../../../matrix.md) is

$$
a(s^2+t^2)+2bst.
$$

Since $a\geq|b|$, both $a$ and $a-|b|$ are nonnegative, and

$$
a(s^2+t^2)+2bst\geq a(s^2+t^2)-2|b||st|
\geq(a-|b|)(s^2+t^2)\geq0.
$$

Equivalently it is

$$
\frac{a+b}{2}(s+t)^2+\frac{a-b}{2}(s-t)^2.
$$

Therefore the [bipartite block-constant positive semidefinite matrix](../../../../../../bipartite-block-constant-positive-semidefinite-matrix.md) satisfies $\boxed{\begin{pmatrix}aJ_{n,n}&bJ_{n,m}\\bJ_{m,n}&aJ_{m,m}\end{pmatrix}\succeq0}$.

For positive block sizes, the condition is also necessary: choose $s=t$ and $s=-t$ to obtain $a+b\geq0$ and $a-b\geq0$. Equality is allowed, and [vectors](../../../../../../vector.md) whose sums vanish in both blocks lie in the [kernel](../../../../../../kernel-of-a-linear-map.md). [Positive semidefiniteness](../../../../../../positive-semidefinite-matrix.md), rather than positive definiteness, is the conclusion.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 339](../../../paper-339-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

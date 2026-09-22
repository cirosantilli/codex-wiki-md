<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let

$$
v=B_{\tau^{-1}f}(z/\tau).
$$

The [proximal operator](../../../../../../proximal-operator.md) optimality condition says

$$
z/\tau-v\in\tau^{-1}\partial f(v),
\quad\text{so}\quad p:=z-\tau v\in\partial f(v).
$$

By [subgradient inversion under convex conjugacy](../../../../../../subgradient-inversion-under-convex-conjugacy.md), which uses [Fenchel–Young inequality](../../../../../../fenchel-young-inequality.md) and $f^{**}=f$ from the [Fenchel-Moreau theorem](../../../../../../fenchel-moreau-theorem.md),

$$
v\in\partial f^*(p).
$$

Consequently $z-p=\tau v\in\tau\partial f^*(p)$, meaning $p=B_{\tau f^*}(z)$. Uniqueness of the [backward subgradient step](../../../../../../proximal-operator.md) identifies the result:

$$
\boxed{B_{\tau f^*}(z)=z-\tau B_{\tau^{-1}f}(z/\tau).}
$$

This is the scaled [Moreau decomposition](../../../../../../moreau-decomposition.md). It requires **one backward step on $f$, with reciprocal parameter $1/\tau$ and scaled input $z/\tau$**, followed by a scalar multiplication and subtraction. No separate proximal computation of the [convex conjugate](../../../../../../convex-conjugate.md) is needed.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 62](../../../paper-62-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

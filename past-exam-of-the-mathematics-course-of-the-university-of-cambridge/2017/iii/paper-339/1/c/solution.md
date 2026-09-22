<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For each fixed $x$ in the [nonnegative orthant](../../../../../../nonnegative-orthant.md), the map $A\mapsto x^TAx$ is a continuous [linear function](../../../../../../linear-function.md) on the [vector space](../../../../../../vector-space-split.md) of real [symmetric matrices](../../../../../../symmetric-matrix.md). Thus

$$
K=\bigcap_{x\geq0}\{A:\langle A,xx^T\rangle_F\geq0\}
$$

is an intersection of [closed half-spaces](../../../../../../closed-half-space.md), using the [Frobenius inner product](../../../../../../frobenius-inner-product.md) $\langle A,B\rangle_F=\operatorname{tr}(AB)$ on this space. Arbitrary intersections of [closed sets](../../../../../../closed-set.md) are closed, so $K$ is closed.

If $A,B\in K$ and $s,t\geq0$, then $x^T(sA+tB)x=sx^TAx+tx^TBx\geq0$ for every $x\geq0$. Therefore $sA+tB\in K$, including the zero [matrix](../../../../../../matrix.md) when $s=t=0$. Hence

$$
\boxed{K\text{ is a closed convex cone}}.
$$

The [copositive cone](../../../../../../copositive-cone.md) is defined in the real space of [symmetric matrices](../../../../../../symmetric-matrix.md); symmetry is needed later to recover every [matrix](../../../../../../matrix.md) entry from these [quadratic forms](../../../../../../quadratic-form.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 339](../../../paper-339-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

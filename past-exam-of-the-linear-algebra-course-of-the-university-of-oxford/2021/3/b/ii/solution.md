<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [ii](../ii.md)

**No.** On the [real vector space](../../../../../real-vector-space.md) $V=\mathbb R^2$, use the [symmetric bilinear form](../../../../../symmetric-bilinear-form.md)

$$
((x,y),(s,t))=xs-yt.
$$

Its [matrix of a bilinear form](../../../../../matrix-of-a-bilinear-form.md) is $\operatorname{diag}(1,-1)$, whose [determinant](../../../../../determinant.md) is $-1\ne0$, so it is a [nondegenerate bilinear form](../../../../../nondegenerate-bilinear-form.md). Let

$$
U=\operatorname{span}\{(1,1)\}.
$$

A [vector](../../../../../vector.md) $(s,t)$ belongs to the [bilinear orthogonal complement](../../../../../orthogonal-complement-for-a-bilinear-form.md) $U^\perp$ exactly when $s-t=0$. Hence

$$
\boxed{U^\perp=U,\qquad U\cap U^\perp=U\ne0,\qquad U+U^\perp=U\ne V.}
$$

In particular, the claimed [direct sum](../../../../../direct-sum.md) fails. The [isotropic vector](../../../../../isotropic-vector.md) $(1,1)$ has zero self-pairing, although it pairs nontrivially with other [vectors](../../../../../vector.md) of $V$.

The [dimension](../../../../../dimension-vector-space.md) identity in part (i) counts both [vector subspaces](../../../../../vector-subspace.md) but does not force their [intersection of vector subspaces](../../../../../intersection-of-vector-subspaces.md) to be zero. For a [symmetric bilinear form](../../../../../symmetric-bilinear-form.md), $U\cap U^\perp$ is the [radical of a bilinear form](../../../../../radical-of-a-bilinear-form.md) restricted to $U$. Thus the precise criterion is

$$
\boxed{V=U\oplus U^\perp\ \Longleftrightarrow\
\text{the restriction of the form to }U\text{ is nondegenerate}.}
$$

Indeed, trivial [intersection of vector subspaces](../../../../../intersection-of-vector-subspaces.md) and part (i) give a [sum of vector subspaces](../../../../../sum-of-vector-subspaces.md) of [dimension](../../../../../dimension-vector-space.md) $\dim V$. A [positive-definite bilinear form](../../../../../positive-definite-bilinear-form.md) would guarantee this for every $U$; symmetry alone does not.

## ↑ Ancestors (13)

1. [ii](../ii.md)
2. [b](../../b.md)
3. [3](../../../3.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the linear algebra course of the University of Oxford](../../../../split.md)
6. [Linear algebra course of the University of Oxford](../../../../../linear-algebra-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

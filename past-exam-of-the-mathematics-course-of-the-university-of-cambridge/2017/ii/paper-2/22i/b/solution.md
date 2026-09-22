<h1 id="22i/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Jacobian criterion](../../../../../../jacobian-criterion.md) on an affine chart $x_j\ne0$ says that a point of the [projective hypersurface](../../../../../../projective-hypersurface.md) is singular exactly when all [derivatives](../../../../../../derivative.md) of its dehomogenized equation vanish there. The [Euler homogeneous function theorem](../../../../../../euler-theorem-for-homogeneous-functions.md) identity $\sum_ix_if_{x_i}=df$ then recovers the omitted $j$th [derivative](../../../../../../derivative.md) on $X$, without dividing by $d$. Thus the correct statement in every characteristic is

$$
\boxed{\operatorname{Sing}(X)=X\cap V(f_{x_0},\ldots,f_{x_n}).}
$$

If the printed $Z(I)$ denotes a zero locus inside $X$, this proves it as written. If it means the ambient projective zero locus, the assertion is false when the characteristic divides $d$. When the characteristic does not divide $d$, the [Euler homogeneous function theorem](../../../../../../euler-theorem-for-homogeneous-functions.md) forces $f=0$ at every common zero of the [derivatives](../../../../../../derivative.md), and the intersection with $X$ is redundant.

For a genuine counterexample to the unrestricted ambient interpretation, in characteristic $p$ take

$$
f=X_0^p+X_1^{p-1}X_2.
$$

This is an irreducible [homogeneous polynomial](../../../../../../homogeneous-polynomial.md): it is primitive and linear in $X_2$ over $k[X_0,X_1]$, with coprime coefficients. At $[1:0:0]$ all [partial derivatives](../../../../../../partial-derivative.md) vanish, including when $p=2$, but $f=1$. This point is outside $X$. Hence **the ambient-locus version needs the displayed intersection or a restriction on the degree**.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [22I](../../22i.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

<h1 id="25f/solution">Solution</h1>

↑ **Parent:** [25F](../25f.md)

For $X\subseteq\mathbb A^n$ and $P\in X$, the [Zariski tangent space](../../../../../zariski-tangent-space.md) is

$$
T_PX=\{v\in k^n:df_P(v)=0\text{ for every }f\in I(X)\}.
$$

The dimension can be defined as $\min_{P\in X}\dim T_PX$. Equivalently, the [krull dimension of an affine variety](../../../../../krull-dimension-of-an-affine-variety.md) is the supremum of lengths of strict chains of irreducible closed subsets, or the Krull dimension of $k[X]$. A point is singular when $\dim T_PX>\dim X$.

For

$$
X=Z(x_1^2-x_2^2,x_3^2-x_4^2),
$$

the differentials give the [tangent spaces of a product of two nodal line pairs](../../../../../tangent-spaces-of-a-product-of-two-nodal-line-pairs.md)

$$
\boxed{T_PX=\{v:x_1v_1-x_2v_2=0,\quad
x_3v_3-x_4v_4=0\}}.
$$

The variety is a union of four two-dimensional linear spaces. If both pairs $(x_1,x_2)$ and $(x_3,x_4)$ are nonzero, the two displayed equations are independent and $\dim T_PX=2$. If exactly one pair is zero, the dimension is three; at the origin it is four. Thus the singular locus is the union of the loci where either coordinate pair vanishes.

For $Y$, rank at most one is equivalent to vanishing of all $2\times2$ minors:

$$
y_0y_3-y_1y_2=0,\qquad
y_0y_4-y_2^2=0,\qquad
y_1y_4-y_2y_3=0.
$$

These homogeneous equations prove that $Y$ is projectively Zariski closed.

The following affine charts show both its dimension and smoothness. On $y_0=1$,

$$
y_3=y_1y_2,\qquad y_4=y_2^2,
$$

so $(y_1,y_2)$ are free. On $y_1=1$,

$$
y_2=y_0y_3,\qquad y_4=y_0y_3^2,
$$

so $(y_0,y_3)$ are free. On $y_3=1$,

$$
y_2=y_1y_4,\qquad y_0=y_1^2y_4,
$$

and on $y_4=1$,

$$
y_1=y_2y_3,\qquad y_0=y_2^2.
$$

These four charts cover $Y$, since the point with only $y_2$ nonzero violates the second minor. Every chart is isomorphic to $\mathbb A^2$. Hence the [smooth projective surface from overlapping rank-one coordinates](../../../../../smooth-projective-surface-from-overlapping-rank-one-coordinates.md) satisfies

$$
\boxed{\dim Y=2}
$$

and is nonsingular everywhere.

## ↑ Ancestors (10)

1. [25F](../25f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

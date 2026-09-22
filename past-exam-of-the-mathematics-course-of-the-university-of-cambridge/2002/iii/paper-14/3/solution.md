<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A subset $X\subset M^m$ is a $d$-dimensional [embedded submanifold](../../../../../embedded-submanifold.md) if, with the subspace topology, every point has a smooth ambient chart in which $X$ is the intersection of the coordinate domain with $\mathbb R^d\times\{0\}$. These slice charts give its smooth structure, and its inclusion is an [embedding](../../../../../embedding.md).

The [inverse function theorem](../../../../../inverse-function-theorem.md) says that a smooth map $F:U\subset\mathbb R^m\to\mathbb R^m$ with invertible derivative at $a$ restricts to a [diffeomorphism](../../../../../diffeomorphism.md) between open neighborhoods of $a$ and $F(a)$. A point $q\in N$ is a [regular value](../../../../../regular-value.md) of a smooth map $f:M^m\to N^n$ when $df_x:T_xM\to T_qN$ is surjective at every $x\in f^{-1}(q)$.

Choose local coordinates centered at $x$ and $q$. At a fiber point, rank $n$ means that, after relabeling coordinates, the first $n$ columns of the coordinate derivative form an invertible [matrix](../../../../../matrix.md). Define

$$
F(u_1,\ldots,u_m)=\bigl(f_1(u),\ldots,f_n(u),u_{n+1},\ldots,u_m\bigr).
$$

Its derivative is block upper triangular with that invertible block and an identity block, hence invertible. The inverse function theorem makes $F$ a new ambient coordinate chart in which $f^{-1}(q)$ is exactly $v_1=\cdots=v_n=0$. Therefore the [regular level set theorem](../../../../../regular-level-set-theorem.md) gives

$$
\boxed{f^{-1}(q)\text{ is an embedded submanifold of dimension }m-n}
$$

when the fiber is nonempty. An empty fiber is regular vacuously; if $m<n$, it is the only possible regular fiber. The construction does not assign a negative dimension to a nonempty manifold.

For the projective hyperplane, the map

$$
\iota:\mathbb{RP}^1\longrightarrow\mathbb{RP}^2,\qquad[a:b]\longmapsto[a:b:0]
$$

is injective with inverse $[x_0:x_1:0]\mapsto[x_0:x_1]$ on its image. At every image point, either $x_0$ or $x_1$ is nonzero; the corresponding standard projective chart uses $x_2/x_i$ as one coordinate and cuts the image out by setting it to zero. The map and inverse are smooth in these charts, and the slice condition proves

$$
\boxed{X\text{ is embedded and }X\cong\mathbb{RP}^1}.
$$

Nevertheless, $\mathbb{RP}^2\setminus X$ is the single affine chart $x_2\ne0$, diffeomorphic to $\mathbb R^2$, so it is connected. If a smooth real function had exactly this zero set with zero regular, the inverse function theorem near any point of $X$ would give both positive and negative values off $X$. On the connected complement it never vanishes, so continuity requires its sign to be constant. This contradiction is the obstruction that [regular zero hypersurfaces have disconnected complements](../../../../../regular-zero-hypersurfaces-have-disconnected-complements.md). Thus

$$
\boxed{X\text{ cannot be a global regular zero set of a smooth real function}}.
$$

It illustrates why local defining equations for an embedded hypersurface need not glue to a global real defining function, as in [real projective hyperplane is not a global regular zero set](../../../../../real-projective-hyperplane-is-not-a-global-regular-zero-set.md).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 14](../../paper-14-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

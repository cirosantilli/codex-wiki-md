<h1 id="25i/solution">Solution</h1>

↑ **Parent:** [25I](../25i.md)

An embedded smooth $d$-dimensional [manifold](../../../../../topological-manifold.md) $X\subset\mathbb R^N$ is locally carried by a smooth ambient coordinate change to $\mathbb R^d\times\{0\}$. A map between such [manifolds](../../../../../topological-manifold.md) is a [smooth map between manifolds](../../../../../smooth-map-between-manifolds.md) if its coordinate representatives are smooth. Its [differential](../../../../../differential-of-a-smooth-map.md) $df_x:T_xX\to T_{f(x)}Y$ sends the tangent vector represented by a curve $\gamma$ to $(f\circ\gamma)'(0)$; equivalently it is the [derivative](../../../../../derivative.md) in charts.

A [regular value](../../../../../regular-value.md) $y$ is one for which $df_x$ is surjective at every $x\in f^{-1}(y)$, including vacuous regularity when the fibre is empty. For example zero is not a [regular value](../../../../../regular-value.md) of $f:\mathbb R\to\mathbb R$, $f(x)=x^2$, because $df_0=0$.

For an invertible [matrix](../../../../../matrix.md) $A$, the [derivative of the determinant](../../../../../derivative-of-the-determinant.md) is

$$
(d\det)_A(H)=\det(A)\operatorname{Tr}(A^{-1}H).
$$

At a determinant-one [matrix](../../../../../matrix.md) it is nonzero, since taking $H=A/n$ gives value one. The [regular level set theorem](../../../../../regular-level-set-theorem.md) therefore makes $SL_n(\mathbb R)=\det^{-1}(1)$ an embedded [manifold](../../../../../topological-manifold.md) of dimension $n^2-1$, also for $n=1$ when it is a single point. [Matrix](../../../../../matrix.md) multiplication has [polynomial](../../../../../polynomial-split.md) ambient coordinates and restricts to the [group](../../../../../group-split.md), so it is smooth. At the identity,

$$
\boxed{T_I SL_n(\mathbb R)=\{H:\operatorname{Tr}H=0\},\qquad\dim SL_n(\mathbb R)=n^2-1}.
$$

Finally suppose the singular-matrix [set](../../../../../set-split.md) were an embedded smooth [manifold](../../../../../topological-manifold.md) near zero for $n\ge2$. Every curve $t\mapsto tE_{ij}$ lies in it, since its rank is at most one. Thus every [matrix](../../../../../matrix.md) unit belongs to its [tangent space](../../../../../tangent-space.md) at zero. These span $\mathbb R^{n^2}$, forcing its local dimension to be $n^2$. An embedded [manifold](../../../../../topological-manifold.md) of full ambient dimension is locally open, but arbitrarily small scalar multiples of the identity are invertible. This contradiction proves **the singular-matrix [set](../../../../../set-split.md) is not an embedded smooth [manifold](../../../../../topological-manifold.md)**. The argument addresses the subset-manifold convention specified at the start.

## ↑ Ancestors (10)

1. [25I](../25i.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

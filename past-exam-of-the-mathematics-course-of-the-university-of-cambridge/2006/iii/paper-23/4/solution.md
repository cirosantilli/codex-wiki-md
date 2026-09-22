<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Take $T$ to be a finite group acting by orientation-preserving [isometries](../../../../../isometry.md). We give both an unbranched construction for every such abstract group and the orbifold construction needed for low-genus examples. The inherited quotient metric and the existence of some unrelated smooth hyperbolic metric on the underlying topological surface are different questions.

For a free action, choose generators $t_1,\ldots,t_s$ of $T$ and a closed orientable surface of genus $g_0\geq\max(2,s)$. Its [surface group](../../../../../fundamental-group-of-a-surface.md) has generators $a_j,b_j$ and relation $\prod_j[a_j,b_j]=1$. Sending $a_j$ to the chosen generators, the remaining $a_j$ to one, and all $b_j$ to one defines a surjective homomorphism to $T$. Its kernel determines a connected regular finite cover $M$. Give the base a [Riemannian metric](../../../../../riemannian-metric.md) of constant curvature $-1$ by the [uniformization theorem](../../../../../uniformization-theorem.md), and pull it back to $M$. Its deck group is $T$, acting freely and isometrically. All subgroup quotients are then smooth covers as well.

For the more general construction, prescribe an oriented compact hyperbolic [orbifold](../../../../../orbifold.md) of signature $(g_0;m_1,\ldots,m_r)$, with

$$
\chi_{\mathrm{orb}}=2-2g_0-\sum_{i=1}^r(1-1/m_i)<0.
$$

Its [orbifold fundamental group](../../../../../orbifold-fundamental-group.md) has presentation

$$
\Gamma=\left\langle a_j,b_j,c_i\ \middle|\ c_i^{m_i}=1,\ \prod_{j=1}^{g_0}[a_j,b_j]c_1\cdots c_r=1\right\rangle.
$$

Choose an epimorphism $\theta:\Gamma\to T$ for which every $\theta(c_i)$ has exact order $m_i$. All finite-order elements of the uniformizing group are conjugate to powers of cone generators, so exact orders make $K=\ker\theta$ torsion-free. Realize $\Gamma$ as a cocompact [Fuchsian group](../../../../../fuchsian-group.md) on the [hyperbolic plane](../../../../../hyperbolic-plane.md). Then

$$
M=K\backslash\mathbb H^2,\qquad M_0=T\backslash M=\Gamma\backslash\mathbb H^2,\qquad M_1=U\backslash M=\theta^{-1}(U)\backslash\mathbb H^2.
$$

The source notation $T/M$ is interpreted as the quotient of $M$ by $T$, as in the consistent subgroup notation $U\backslash M$. The manifold $M$ is smooth; $M_0$ has cone angles $2\pi/m_i$ and may have singularities.

The [smoothness criterion from cone-monodromy cycles](../../../../../smoothness-criterion-from-cone-monodromy-cycles.md) is explicit. On the $n=[T:U]$ cosets, let $\sigma_i$ be the permutation induced by $\theta(c_i)$. A cycle of length $\ell$ has local degree $\ell$ over the cone point. The resulting total angle is $2\pi\ell/m_i$, so its residual cone order is $m_i/\ell$. Therefore the inherited metric on $M_1$ is smooth precisely when every cycle of every $\sigma_i$ has length $m_i$. Equivalently,

$$
U\cap t\langle\theta(c_i)\rangle t^{-1}=\{1\}\qquad\text{for every }t\in T\text{ and every }i.
$$

Indeed a nonidentity cone-generator power fixes a coset exactly when its conjugate lies in $U$. The inherited metric on $M_0$ itself is smooth precisely when there are no nontrivial cone stabilizers, equivalently when the $T$ action on $M$ is free.

For the [Euler characteristics](../../../../../euler-characteristic.md), first distinguish the ordinary characteristic of the underlying base from its [orbifold Euler characteristic](../../../../../orbifold-euler-characteristic.md):

$$
\boxed{\chi(|M_0|)=2-2g_0,\qquad\chi_{\mathrm{orb}}(M_0)=2-2g_0-r+\sum_i\frac1{m_i}.}
$$

To derive the covering formulas, triangulate the underlying base with all cone points as vertices. Ordinary vertices, open edges and faces lift with their full degree. A cone point whose monodromy has $c_i$ cycles has $c_i$ preimage vertices rather than $n$; thus the lifted Euler characteristic loses $n-c_i$ there. This is the [Euler characteristic from coset cycle counts](../../../../../euler-characteristic-from-coset-cycle-counts.md):

$$
\chi(|M_1|)=n\chi(|M_0|)-\sum_i(n-c_i)=n(2-2g_0-r)+\sum_i c_i.
$$

For the full regular cover $M$, each cone generator acts on $T$ in cycles of length $m_i$, so it has $|T|/m_i$ cycles. Consequently

$$
\boxed{\chi(M)=|T|\left(2-2g_0-r+\sum_i\frac1{m_i}\right).}
$$

When $M_1$ is smooth, all its cone cycles likewise have full length and $c_i=n/m_i$. Hence

$$
\boxed{\chi(M_1)=[T:U]\left(2-2g_0-r+\sum_i\frac1{m_i}\right)=\frac{\chi(M)}{|U|}.}
$$

These are also the [Riemann-Hurwitz formula](../../../../../riemann-hurwitz-formula.md) with the ramification deficits made explicit. The [Gauss-Bonnet theorem](../../../../../gauss-bonnet-theorem.md) gives area $-2\pi\chi$ for each smooth closed hyperbolic surface, consistently multiplying with covering degree.

Finally, if one asks whether the underlying surface admits any smooth metric of constant curvature $-1$, rather than whether this quotient metric is smooth, the criterion is ordinary [Euler characteristic](../../../../../euler-characteristic.md) less than zero. Necessity follows from the [Gauss-Bonnet theorem](../../../../../gauss-bonnet-theorem.md); sufficiency is the [uniformization theorem](../../../../../uniformization-theorem.md) for genus at least two. Thus an orbifold quotient with cone singularities can sometimes be given a different smooth hyperbolic metric, but this change does not preserve its role as the locally isometric quotient in the spectral construction. A sphere or torus underlying $M_0$ cannot be made a closed smooth curvature-$-1$ surface at all.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 23](../../paper-23-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

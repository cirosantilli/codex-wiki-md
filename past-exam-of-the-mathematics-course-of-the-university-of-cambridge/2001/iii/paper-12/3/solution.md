<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use the [Levi-Civita connection](../../../../../levi-civita-connection.md) $\nabla$ of the [Riemannian metric](../../../../../riemannian-metric.md) $g$ and fix the convention

$$
R(X,Y)Z=\nabla_X\nabla_YZ-\nabla_Y\nabla_XZ-\nabla_{[X,Y]}Z,\qquad R_4(X,Y,Z,W)=g(R(X,Y)Z,W).
$$

The [Leibniz rule](../../../../../leibniz-rule.md) shows that this expression is linear over smooth functions in all three arguments: the differentiated coefficient terms in the first two derivatives cancel those in the bracket term. Thus $R$ is a section of $\Lambda^2T^*M\otimes\operatorname{End}(TM)$, the [Riemann curvature tensor](../../../../../riemann-curvature-tensor.md), and $R_4$ is a covariant [tensor field](../../../../../tensor-field.md). This convention gives positive [sectional curvature](../../../../../sectional-curvature.md) on the round sphere.

Its algebraic symmetries are

$$
\begin{aligned}
R_4(X,Y,Z,W)&=-R_4(Y,X,Z,W),\\
R_4(X,Y,Z,W)&=-R_4(X,Y,W,Z),\\
R(X,Y)Z+R(Y,Z)X+R(Z,X)Y&=0,\\
R_4(X,Y,Z,W)&=R_4(Z,W,X,Y).
\end{aligned}
$$

The first identity follows immediately from the definition. For the second, apply $XY-YX-[X,Y]$ to $g(Z,W)$ and use compatibility of the [Levi-Civita connection](../../../../../levi-civita-connection.md) with the [Riemannian metric](../../../../../riemannian-metric.md). The left side is zero and the differentiated terms combine to

$$
g(R(X,Y)Z,W)+g(Z,R(X,Y)W)=0.
$$

For the [first Bianchi identity](../../../../../first-bianchi-identity.md), use [normal coordinates](../../../../../normal-coordinates.md) at a point $p$, so the [Christoffel symbols](../../../../../christoffel-symbol.md) vanish there. Torsion-freeness gives $\Gamma^\ell_{ij}=\Gamma^\ell_{ji}$, and

$$
R(\partial_i,\partial_j)\partial_k\big|_p
=(\partial_i\Gamma^\ell_{jk}-\partial_j\Gamma^\ell_{ik})\partial_\ell\big|_p.
$$

The cyclic sum over $i,j,k$ cancels term by term. Since this is a tensor identity, it holds for arbitrary tangent vectors everywhere.

To prove pair interchange rather than assume it, abbreviate $R_4(a,b,c,d)$ to $R_{abcd}$ and put $A=R_{abcd}$, $B=R_{cdab}$. The [first Bianchi identity](../../../../../first-bianchi-identity.md) and the two antisymmetries give

$$
A=R_{bcda}+R_{cadb}
=2B-R_{dbca}-R_{adcb}.
$$

The [first Bianchi identity](../../../../../first-bianchi-identity.md) applied to $(d,b,a)$ with final argument $c$ gives $R_{dbca}+R_{adcb}=R_{badc}=A$. Hence $A=2B-A$, proving $A=B$.

There is also the differential [second Bianchi identity](../../../../../second-bianchi-identity.md),

$$
(\nabla_XR)(Y,Z)+(\nabla_YR)(Z,X)+(\nabla_ZR)(X,Y)=0.
$$

For its proof take commuting coordinate fields, normal at $p$. The [Jacobi identity](../../../../../jacobi-identity.md) for operator commutators says $[\nabla_X,[\nabla_Y,\nabla_Z]]+\text{cyclic}=0$. On these commuting fields, $[\nabla_Y,\nabla_Z]=R(Y,Z)$; at $p$, the covariant derivatives of the coordinate arguments vanish. The commutator identity is therefore the displayed covariant derivative identity at $p$, and tensoriality establishes it everywhere.

For a two-dimensional plane $\sigma=\operatorname{span}\{X,Y\}\subset T_pM$, define the [sectional curvature](../../../../../sectional-curvature.md) by

$$
\boxed{K(\sigma)=\frac{g(R(X,Y)Y,X)}{|X|^2|Y|^2-g(X,Y)^2}.}
$$

The denominator is the squared area of $X,Y$. Under an invertible change of plane basis, the alternating pairs in the numerator and the area in the denominator both acquire the square of the change-of-basis determinant. Thus the quotient depends only on $\sigma$. For an [orthonormal basis](../../../../../orthonormal-basis.md) of $\sigma$, it is simply $g(R(X,Y)Y,X)$.

The [Ricci curvature](../../../../../ricci-curvature.md) is the trace

$$
\operatorname{Ric}(X,Y)=\operatorname{tr}\{Z\mapsto R(Z,X)Y\}
=\sum_{i=1}^n g(R(e_i,X)Y,e_i),
$$

where $(e_i)$ is any [orthonormal basis](../../../../../orthonormal-basis.md) of $T_pM$. This is independent of the basis because it is a trace. Applying the [first Bianchi identity](../../../../../first-bianchi-identity.md) to $(e_i,X,Y)$ and pairing with $e_i$ proves that the summand difference for $\operatorname{Ric}(X,Y)-\operatorname{Ric}(Y,X)$ vanishes; the middle term $g(R(X,Y)e_i,e_i)$ is zero by the last-pair antisymmetry. Hence [Ricci curvature](../../../../../ricci-curvature.md) is a symmetric bilinear form. For a unit vector $v=e_1$ extended to an [orthonormal basis](../../../../../orthonormal-basis.md),

$$
\boxed{\operatorname{Ric}(v,v)=\sum_{i=2}^n K(\operatorname{span}\{v,e_i\}).}
$$

For nonzero $X$, take $v=X/|X|$ and multiply the right side by $|X|^2$. This determines the entire [Ricci curvature](../../../../../ricci-curvature.md) by the [polarization identity](../../../../../polarization-identity.md):

$$
\operatorname{Ric}(X,Y)=\tfrac14\bigl(\operatorname{Ric}(X+Y,X+Y)-\operatorname{Ric}(X-Y,X-Y)\bigr).
$$

Finally, the [scalar curvature](../../../../../scalar-curvature.md) is the metric trace of [Ricci curvature](../../../../../ricci-curvature.md). Taking its diagonal entries in an [orthonormal basis](../../../../../orthonormal-basis.md) and pairing the equal contributions from $(i,j)$ and $(j,i)$ yields

$$
\boxed{\operatorname{Scal}=\sum_i\operatorname{Ric}(e_i,e_i)=2\sum_{1\leq i<j\leq n}K(\operatorname{span}\{e_i,e_j\}).}
$$

In particular, constant [sectional curvature](../../../../../sectional-curvature.md) $K_0$ gives $\operatorname{Ric}=(n-1)K_0g$ and $\operatorname{Scal}=n(n-1)K_0$. In dimension one the traces are zero; there are no two-dimensional tangent planes and the sums are empty.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 12](../../paper-12-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

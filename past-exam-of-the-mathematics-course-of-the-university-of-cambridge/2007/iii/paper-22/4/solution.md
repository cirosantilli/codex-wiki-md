<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Choose [holomorphic coordinates](../../../../../holomorphic-coordinate.md) centered at the point $p$ and a [polydisc](../../../../../polydisc.md) $U\subset\mathbb C^n$ about the origin. The local [blowup of a complex manifold at a point](../../../../../blowup-of-a-complex-manifold-at-a-point.md) is the incidence manifold

$$
\widetilde U=\{(z,[\ell])\in U\times\mathbb{CP}^{n-1}:z_i\ell_j=z_j\ell_i\text{ for all }i,j\},
\qquad\sigma(z,[\ell])=z.
$$

Away from $z=0$ the direction is forced to be $[\ell]=[z]$, giving a [biholomorphism](../../../../../biholomorphism.md) with $U\setminus\{0\}$. Glue this punctured part to $X\setminus\{p\}$. The charts below make the result a [complex manifold](../../../../../complex-manifold.md). The projection is proper near $p$, since it is the restriction of projection from a closed subset of $U\times\mathbb{CP}^{n-1}$; globally the modification is proper and is an isomorphism off $p$. Its [exceptional divisor](../../../../../exceptional-divisor.md) is

$$
E=\sigma^{-1}(p)\cong\mathbb P(T_pX)\cong\mathbb{CP}^{n-1}.
$$

On $\ell_i\ne0$, let $t=z_i$ and $u_j=\ell_j/\ell_i$ for $j\ne i$. Then

$$
z_i=t,\qquad z_j=t u_j\ (j\ne i).
$$

These are coordinates on the open domain where $t$ and all $t u_j$ lie in the original polydisc; at $t=0$ all finite $u_j$ are allowed. Their inverse reads the direction ratios and $z_i$ from the incidence point. In this chart $E$ is the nonsingular hypersurface $t=0$. On overlap with chart $k\ne i$, the [holomorphic coordinate](../../../../../holomorphic-coordinate.md) changes are

$$
t'=t u_k,\qquad u'_i=1/u_k,\qquad u'_j=u_j/u_k\quad(j\ne i,k).
$$

They are holomorphic with holomorphic inverses where $u_k\ne0$, and the $n$ charts cover every point of $E$. Intrinsically, changing the original coordinates by $F$ lifts via $[\ell]\mapsto[A(z)\ell]$, where $F(z)=A(z)z$, $A(0)=dF_0$, and $A$ is holomorphic and invertible near zero. One can take $A(z)=\int_0^1dF_{sz}\,ds$ on a sufficiently small polydisc. Away from the origin the lift is uniquely forced; this proves coordinate-independence of the gluing near $E$.

The [canonical bundle](../../../../../canonical-bundle.md) is $K_X=\Lambda^n\Omega_X^1$. In the $i$th blowup chart the top-form Jacobian is

$$
\sigma^*(dz_1\wedge\cdots\wedge dz_n)
=(-1)^{i-1}t^{n-1}\,dt\wedge\bigwedge_{j\ne i}du_j,
$$

where the $u_j$ occur in increasing order. Every term with a second $dt$ vanishes in the [wedge product of differential forms](../../../../../wedge-product-of-differential-forms.md). Thus the differential gives a map $\sigma^*K_X\to K_{\widetilde X}$ vanishing to order $n-1$ along $E$ and nowhere else. To express this through the supplied meromorphic-section hypothesis, take a nonzero meromorphic section $s$ of $K_X$ and put $D=\operatorname{div}(s)$. Locally $s=f(z)\,dz_1\wedge\cdots\wedge dz_n$, so

$$
\operatorname{div}(\sigma^*s)=\sigma^*D+(n-1)E.
$$

Here $\sigma^*D$ is the total divisor pullback, including any additional exceptional multiplicity from $f$; it is not merely the strict transform. A line bundle with a nonzero meromorphic section is isomorphic to the line bundle of that section's divisor, as its local coefficient ratios are its frame transitions. Pullback of divisor line bundles and [additivity of analytic divisor line bundles](../../../../../additivity-of-analytic-divisor-line-bundles.md) therefore give the [canonical bundle formula for a point blowup](../../../../../canonical-bundle-formula-for-a-point-blowup.md):

$$
\boxed{K_{\widetilde X}\cong\sigma^*K_X\otimes\mathcal O_{\widetilde X}((n-1)E).}
$$

For $n=1$ the blowup is already an isomorphism, consistently with the zero exponent.

For the projective-plane construction, an invertible linear change of homogeneous coordinates puts $x=[1:0:0]$. Lines through $x$ are parametrized by $[a:b]\in\mathbb{CP}^1$, with equation $bZ_1-aZ_2=0$. Thus the required map on the punctured plane is

$$
f([Z_0:Z_1:Z_2])=[Z_1:Z_2].
$$

It is well-defined under rescaling and holomorphic on the covering sets $Z_1\ne0$ and $Z_2\ne0$, where its target coordinates are $Z_2/Z_1$ and $Z_1/Z_2$. These sets cover the complement of $x$.

The graph closure is

$$
S=\{([Z_0:Z_1:Z_2],[a:b])\in\mathbb{CP}^2\times\mathbb{CP}^1:Z_1b=Z_2a\}.
$$

Over the complement of $x$ it is the graph of $f$. In the affine chart $Z_0\ne0$, its equation is exactly the two-dimensional local incidence model for the [blowup of a complex manifold at a point](../../../../../blowup-of-a-complex-manifold-at-a-point.md), so its first projection identifies it with the required blowup globally. The second projection is a [holomorphic map](../../../../../holomorphic-map.md) $\widetilde f:S\to\mathbb{CP}^1$ extending $f\circ\sigma$. Explicitly, the two blowup charts give

$$
(z_1,z_2)=(t,tu):\ \widetilde f=[1:u],\qquad
(z_1,z_2)=(tv,t):\ \widetilde f=[v:1].
$$

These formulas agree when $v=1/u$ and remain holomorphic at $t=0$. Hence **the pencil extends over the exceptional divisor, where it records the projective tangent direction**. This is the [projective pencil resolved by a point blowup](../../../../../projective-pencil-resolved-by-a-point-blowup.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 22](../../paper-22-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

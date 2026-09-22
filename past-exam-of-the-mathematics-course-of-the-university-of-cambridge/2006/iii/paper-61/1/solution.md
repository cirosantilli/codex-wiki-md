<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use the paper's curvature convention throughout, and define the [Ricci tensor](../../../../../ricci-tensor.md) and [scalar curvature](../../../../../scalar-curvature.md) by $R_{kn}=R^i{}_{kin}$ and $R=g^{kn}R_{kn}$. In particular, if semicolons are read from left to right, $X^i{}_{;km}=\nabla_m(\nabla_kX)^i$, including the connection on the derivative index. This ordering matters for the [Ricci identity](../../../../../curvature-commutator-on-a-covariant-tensor.md) sign.

Choose [Riemann normal coordinates](../../../../../normal-coordinates.md) at an arbitrary point $P$. The [Christoffel symbols](../../../../../christoffel-symbol.md) vanish there, and the [Levi-Civita connection](../../../../../levi-civita-connection.md) formula gives

$$
R_{ikmn}(P)=\frac12\left(g_{im,kn}+g_{kn,im}-g_{km,in}-g_{in,km}\right)(P).
$$

Metric symmetry and commuting partial derivatives show directly that exchanging $m,n$ or $i,k$ changes the sign, while interchanging the pairs $(i,k)$ and $(m,n)$ leaves the expression unchanged. Adding its three cyclic versions over $k,m,n$ cancels every second derivative. These are tensorial statements and $P$ was arbitrary, so

$$
\boxed{R^i{}_{k(mn)}=0,\qquad R^i{}_{[kmn]}=0,\qquad R_{(ik)mn}=0,\qquad R_{ikmn}=R_{mnik}.}
$$

The cyclic relation is the [first Bianchi identity](../../../../../first-bianchi-identity.md); its reduction to the total antisymmetrization uses last-pair antisymmetry. These arguments use zero [torsion tensor](../../../../../torsion-tensor.md) and [metric compatibility](../../../../../metric-compatibility.md), not a field equation.

At $P$, the [covariant derivative](../../../../../covariant-derivative.md) of curvature equals its partial derivative. Differentiating the connection expression for curvature gives derivatives of $\partial_n\Gamma^i{}_{km}-\partial_m\Gamma^i{}_{kn}$; derivatives of the quadratic connection terms vanish because $\Gamma(P)=0$. In the cyclic sum over $m,n,p$, every second derivative of a connection coefficient occurs twice with opposite signs. Thus

$$
R^i{}_{kmn;p}+R^i{}_{knp;m}+R^i{}_{kpm;n}=0,
\qquad\boxed{R^i{}_{k[mn;p]}=0.}
$$

This is the [second Bianchi identity](../../../../../second-bianchi-identity.md), valid everywhere by tensoriality.

Lower the first curvature index and contract the differential identity with $g^{im}$. [Metric compatibility](../../../../../metric-compatibility.md) allows the metric to pass through the [covariant derivatives](../../../../../covariant-derivative.md). Using the pair antisymmetries yields

$$
\boxed{\nabla^iR_{ikmn}=\nabla_mR_{kn}-\nabla_nR_{km}.}
$$

Contract again with $g^{km}$. The left side is $-\nabla^iR_{in}$, while the right side is $\nabla^kR_{kn}-\nabla_nR$. Hence the [contracted Bianchi identity](../../../../../contracted-bianchi-identity.md) is

$$
\boxed{\nabla^iR_{in}=\frac12\nabla_nR,\qquad
\nabla^i\left(R_{in}-\frac12g_{in}R\right)=0.}
$$

The [Ricci tensor](../../../../../ricci-tensor.md) is symmetric, as follows by contracting the pair-exchange symmetry. The final divergence is that of the [Einstein tensor](../../../../../einstein-tensor.md).

For the vector commutator, at the same normal-coordinate point,

$$
X^i{}_{;km}=\partial_m\partial_kX^i+(\partial_m\Gamma^i{}_{jk})X^j.
$$

The terms involving undifferentiated connection coefficients vanish at $P$. Subtracting the reversed expression leaves $(\Gamma^i{}_{jk,m}-\Gamma^i{}_{jm,k})X^j$, exactly the stated curvature convention at $P$. Therefore

$$
\boxed{X^i{}_{;km}-X^i{}_{;mk}=R^i{}_{jkm}X^j.}
$$

For a [covector field](../../../../../one-form.md), its connection term has the opposite sign: $\omega_{i;k}=\partial_k\omega_i-\Gamma^j{}_{ik}\omega_j$. The same calculation gives

$$
\boxed{\omega_{i;km}-\omega_{i;mk}=-R^j{}_{ikm}\omega_j.}
$$

Equivalently, apply the commutator to the scalar $\omega_iX^i$, whose two [covariant derivatives](../../../../../covariant-derivative.md) commute, and cancel the vector contribution. Each covariant index contributes a negative curvature action and each contravariant index a positive one in this semicolon ordering.

To prove the requested [double divergence of the Riemann tensor](../../../../../double-divergence-of-the-riemann-tensor.md), let

$$
D_{mn}=R^{ik}{}_{mn;ik}=\nabla_k\nabla_iR^{ik}{}_{mn}.
$$

The once-contracted identity gives

$$
D_{mn}=\nabla_k\nabla_mR^k{}_n-\nabla_k\nabla_nR^k{}_m.
$$

Commuting the outer derivative past $\nabla_m$ and $\nabla_n$ leaves a difference of scalar Hessians, $\tfrac12(\nabla_m\nabla_n-\nabla_n\nabla_m)R=0$, plus curvature terms. The operator commutator $[\nabla_k,\nabla_m]$ has the negative of the paper's curvature sign, since it reverses the semicolon order. On the mixed [Ricci tensor](../../../../../ricci-tensor.md) it gives

$$
[\nabla_k,\nabla_m]R^k{}_n
=-R_{am}R^a{}_n+R^a{}_{nkm}R^k{}_a.
$$

The first term is symmetric in $m,n$: it is the metric contraction of two symmetric [Ricci tensors](../../../../../ricci-tensor.md). The second is $S_{mn}=R^{ak}R_{ankm}$ and is also symmetric, since

$$
S_{mn}=R^{ak}R_{kman}=R^{ak}R_{amkn}=S_{nm},
$$

where the first equality uses curvature pair exchange and the second swaps the dummy indices $a,k$. Thus the two commutator terms cancel on antisymmetrization in $m,n$, proving

$$
\boxed{R^{ik}{}_{mn;ik}=0.}
$$

No assumption such as vacuum, constant curvature or vanishing [Ricci tensor](../../../../../ricci-tensor.md) was used.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 61](../../paper-61-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

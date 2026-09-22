<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Write $MU^*=\Omega_U^*$ for [complex cobordism](../../../../../complex-cobordism.md). A [complex orientation of a smooth map](../../../../../complex-orientation-of-a-smooth-map.md) is chosen stable complex normal data, not a complex structure on either manifold separately. More concretely, replace the continuous map by a homotopic smooth map $f_0$, choose an embedding

$$
j=(f_0,e):X\hookrightarrow Y\times\mathbb R^N,
$$

and give its [normal bundle](../../../../../normal-bundle.md) $\nu_j$ a [stable complex structure on a real vector bundle](../../../../../stable-complex-structure-on-a-real-vector-bundle.md). The auxiliary dimension can be chosen so the normal rank is even; further stabilization makes the [normal bundle](../../../../../normal-bundle.md) actually complex. Equivalence means stabilization by trivial complex summands and homotopy of the oriented embedding data. The stable identity

$$
\nu_j\oplus TX\cong f_0^*TY\oplus\mathbb R^N
$$

identifies this as orientation of the relative stable [normal bundle](../../../../../normal-bundle.md). For odd relative codimension one uses an odd auxiliary suspension coordinate; the degree formula below is unchanged. This is the geometric factorization model for complex-oriented maps used in [Algebraic and Geometric Topology 18, geometric cobordism discussion](https://msp.org/agt/2018/18-7/agt-v18-n7-p.pdf).

Let $d=\dim Y-\dim X$ and $r=\operatorname{rank}_{\mathbb R}\nu_j=d+N$. The chosen normal orientation gives a [Thom class](../../../../../thom-class.md) $u_{\nu_j}$ of degree $r$ and the [Thom isomorphism in complex cobordism](../../../../../thom-isomorphism-in-complex-cobordism.md). For compact manifolds the [Pontryagin-Thom collapse](../../../../../pontryagin-thom-collapse.md) of a [tubular neighborhood](../../../../../tubular-neighborhood.md) to its [Thom space](../../../../../thom-space.md) is

$$
c_j:Y_+\wedge S^N\longrightarrow\operatorname{Th}(\nu_j).
$$

For $a\in MU^q(X)$, define the [Gysin map in complex cobordism](../../../../../gysin-map-in-complex-cobordism.md) by the composite

$$
MU^q(X)\xrightarrow{\ a\mapsto\pi^*a\,u_{\nu_j}\ }
\widetilde{MU}^{q+r}(\operatorname{Th}(\nu_j))
\xrightarrow{\ c_j^*\ }
\widetilde{MU}^{q+r}(Y_+\wedge S^N)
\xrightarrow{\ \text{desuspension}\ }
MU^{q+d}(Y).
$$

Thus **$f_!$ raises degree by the real relative codimension $d$**. This definition depends on the specified orientation and is invariant under the stated equivalences of its normal data. The plus sign on a space denotes adjoining a disjoint basepoint.

For the embedding $i:L\hookrightarrow M$ with normal rank $2n$, let $c:M_+\to\operatorname{Th}(\nu)$ be its tubular collapse. The Thom construction gives $i_!(1)=c^*u_\nu$. Restricted to $L$, this collapse is exactly the [zero section](../../../../../zero-section-of-a-vector-bundle.md) $z:L\to\operatorname{Th}(\nu)$. Therefore

$$
\boxed{i^*i_!(1)=z^*u_\nu=e_{MU}(\nu)\in MU^{2n}(L).}
$$

This is the [self-intersection formula in complex cobordism](../../../../../self-intersection-formula-in-complex-cobordism.md). For an actual complex rank-$n$ [normal bundle](../../../../../normal-bundle.md) its top [Chern class in complex cobordism](../../../../../chern-class-in-complex-cobordism.md) is the zero-section pullback of its [Thom class](../../../../../thom-class.md), so the right side is $c_n^{MU}(\nu)$. Equivalently, under the [splitting principle for complex vector bundles](../../../../../splitting-principle-for-complex-vector-bundles.md) both are the product of the first [Chern classes](../../../../../chern-class.md) of the line summands. The same argument gives $i^*i_!(a)=a\,e_{MU}(\nu)$ for every $a$.

There is a real distinction if the printed word “stable” is interpreted literally. The [Euler class](../../../../../euler-class-of-a-vector-bundle.md) of a stably complex real bundle need not equal $c_n^{MU}$ of its stable complex class. For the diagonal embedding $S^4\hookrightarrow S^4\times S^4$, the [normal bundle](../../../../../normal-bundle.md) is $TS^4$. It has a stable complex structure with

$$
TS^4\oplus\mathbb R^2\cong\mathbb R^6\cong\mathbb C^3,
$$

so its stable complex rank-two class is trivial and has second [Chern class](../../../../../chern-class.md) zero. However the ordinary integral image of $i^*i_!(1)$ is $e(TS^4)$, which evaluates to the [Euler characteristic](../../../../../euler-characteristic.md) $2$. Thus the always-valid answer is the cobordism [Euler class](../../../../../euler-class-of-a-vector-bundle.md). The requested top-Chern identification is valid for an actual complex [normal bundle](../../../../../normal-bundle.md), or if “top [Chern class](../../../../../chern-class.md)” here is explicitly being used as the Euler-class terminology for the chosen normal orientation.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 19](../../paper-19-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

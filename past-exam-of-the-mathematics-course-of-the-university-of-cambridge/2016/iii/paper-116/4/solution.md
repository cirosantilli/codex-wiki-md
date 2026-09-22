<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Take the normalization

$$
E(\alpha)=\frac12\int_0^1|\dot\alpha(t)|^2\,dt.
$$

The [first variation of geodesic energy](../../../../../first-variation-of-geodesic-energy.md) says that the [critical points](../../../../../critical-point.md) on the fixed-endpoint [path space](../../../../../path-space.md) are exactly the affinely parametrized [geodesics](../../../../../geodesic.md). The kernel of the [second variation of geodesic energy](../../../../../second-variation-of-geodesic-energy.md), or [Riemannian index form](../../../../../riemannian-index-form.md), is the space of [Jacobi fields](../../../../../jacobi-field.md) vanishing at both endpoints. Hence a geodesic is a [nondegenerate critical point](../../../../../nondegenerate-critical-point.md) exactly when that space is zero, or equivalently when its terminal endpoint is not a [conjugate point](../../../../../conjugate-point.md) to its initial endpoint along the given geodesic.

The [Morse index theorem](../../../../../morse-index-theorem.md) states that the index is the sum of the multiplicities of all [conjugate points](../../../../../conjugate-points.md) strictly inside the parameter interval:

$$
\boxed{\operatorname{ind}(\gamma)=\sum_{0<t<1}\dim\{J\in\mathcal J_\gamma:J(0)=J(t)=0\}.}
$$

The multiplicity at the terminal endpoint gives nullity rather than an additional contribution to the index. These statements use the usual Sobolev $H^1$ completion of the [path space](../../../../../path-space.md); smooth paths have the same homotopy type.

First suppose $p\ne q$ as well as $p\ne -q$, and put $\theta=d(p,q)\in(0,\pi)$. There is a unique [great circle](../../../../../great-circle.md) through these two points. Every critical path runs along it with constant speed, possibly passing around it extra times. If

$$
e=\frac{q-(\cos\theta)p}{\sin\theta},
$$

then a complete enumeration without repetitions is

$$
\gamma_\ell(t)=\cos(\ell t)p+\sin(\ell t)e,\qquad \ell=\theta+2\pi m,\quad m\in\mathbb Z.
$$

Its length is $L=|\ell|$. Equivalently the two positive length lists are

$$
L^+_r=\theta+2\pi r,\qquad L^-_r=2\pi-\theta+2\pi r,\qquad r=0,1,2,\ldots.
$$

There are no other critical paths, because a nonconstant [geodesic](../../../../../geodesic.md) of the round [sphere](../../../../../sphere.md) is a constant-speed [great circle](../../../../../great-circle.md) and its plane must contain $p,q$.

To compute [conjugate points and indices of round-sphere geodesics](../../../../../conjugate-points-and-indices-of-round-sphere-geodesics.md), the round unit [sphere](../../../../../sphere.md) has constant [sectional curvature](../../../../../sectional-curvature.md) $1$. Along a geodesic of speed $L$, a normal [Jacobi field](../../../../../jacobi-field.md) in a parallel direction satisfies $y''+L^2y=0$. A field with $J(0)=0$ is therefore a constant multiple of $\sin(Lt)$ in each of the $n-1$ normal directions. Its tangential component satisfies $y''=0$ and contributes no endpoint-vanishing field. Consequently the [conjugate points](../../../../../conjugate-points.md) occur at $Lt=j\pi$, each with multiplicity $n-1$. Since neither length list contains an integer multiple of $\pi$, all the displayed critical paths are nondegenerate, and the [Morse index theorem](../../../../../morse-index-theorem.md) gives

$$
\boxed{\operatorname{ind}(\gamma^+_r)=2r(n-1),\qquad\operatorname{ind}(\gamma^-_r)=(2r+1)(n-1).}
$$

The permitted case $p=q$ requires separate treatment. There is a constant geodesic, which has index and nullity zero. All other critical paths are

$$
\gamma_{r,v}(t)=\cos(2\pi rt)p+\sin(2\pi rt)v,
\qquad r\geq1,\quad v\in T_pS^n,\ |v|=1.
$$

For each $r$, this is a family parametrized by $S^{n-1}$; both directions of traversal are included through $v$ and $-v$. The interior [conjugate points](../../../../../conjugate-points.md) number $2r-1$, and the endpoint is also conjugate. Thus

$$
\boxed{\operatorname{ind}(\gamma_{r,v})=(2r-1)(n-1),\qquad\operatorname{nullity}(\gamma_{r,v})=n-1.}
$$

These are [Morse-Bott critical manifolds](../../../../../morse-bott-critical-manifold.md) for $n>1$, rather than nondegenerate critical points. For $n=1$ the same formulas give zero index and nullity, with the two isolated directions comprising $S^0$.

For the requested [homology](../../../../../homology-split.md) calculation, choose distinct nonantipodal endpoints. Concatenation with a fixed path back to the basepoint gives a [homotopy equivalence](../../../../../homotopy-equivalence.md) between this fixed-endpoint [path space](../../../../../path-space.md) and the based [loop space](../../../../../loop-space.md) $\Omega S^n$. We use the [Morse cell-attachment theorem for geodesic energy](../../../../../morse-cell-attachment-theorem-for-geodesic-energy.md): on a complete compact [Riemannian manifold](../../../../../riemannian-manifold.md), the fixed-endpoint energy, when all its critical points are nondegenerate, gives a [CW complex](../../../../../cw-complex.md) of the same homotopy type with one cell of dimension equal to the index of each critical point. One can obtain this theorem from finite-dimensional broken-geodesic approximations and ordinary [Morse theory](../../../../../morse-theory.md); critical energy values tend to infinity here.

The two index lists interleave to give exactly one cell in every dimension $j(n-1)$, $j\geq0$. If $n>2$, these dimensions are separated by at least two. The [cellular homology](../../../../../cellular-chain-complex.md) groups therefore have zero boundary maps, since no occupied cell dimension has an occupied dimension one lower. With integer coefficients,

$$
\boxed{H_d(\Omega S^n;\mathbb Z)\cong
\begin{cases}
\mathbb Z,&d=j(n-1),\quad j=0,1,2,\ldots,\\
0,&\text{otherwise}.
\end{cases}}
$$

This determines the graded abelian groups. The argument does not need an identification of the multiplication on [loop-space homology](../../../../../loop-space-homology.md).

Finally apply the [Freudenthal suspension theorem](../../../../../freudenthal-suspension-theorem.md): for an $(n-1)$-connected based [CW complex](../../../../../cw-complex.md) $X$, $n\geq2$, the suspension homomorphism

$$
\pi_k(X)\longrightarrow\pi_{k+1}(\Sigma X)
$$

is an isomorphism for $k\leq2n-2$ and a surjection for $k=2n-1$. A [sphere](../../../../../sphere.md) $S^n$ is $(n-1)$-connected, and its reduced [suspension of a topological space](../../../../../suspension-topology.md) is homeomorphic to $S^{n+1}$. Hence

$$
\boxed{\pi_k(S^n)\cong\pi_{k+1}(S^{n+1})\quad(k\leq2n-2).}
$$

The isomorphism is the suspension map. Its stable range is also reflected by the [Morse theory](../../../../../morse-theory.md) cell structure of $\Omega S^{n+1}$: after its bottom $n$-cell, the next positive-dimensional cell has dimension $2n$. For the stated homology problem $n>2$, all the connectivity hypotheses apply.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 116](../../paper-116-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Fix $p$ in a [Riemannian manifold](../../../../../riemannian-manifold.md) $(M,g)$. The preliminary results used are the existence of the [Levi-Civita connection](../../../../../levi-civita-connection.md), which is metric-compatible and torsion-free; local existence, uniqueness and smooth dependence for the geodesic ordinary differential equation; and the [inverse function theorem](../../../../../inverse-function-theorem.md). The local geodesic equation is

$$
\ddot x^i+\Gamma^i{}_{jk}(x)\dot x^j\dot x^k=0,
$$

so these ordinary differential equation results apply to the initial data $(p,v)$. On an open neighborhood of $0\in T_pM$, the solution $\gamma_v$ with $\gamma_v(0)=p$, $\dot\gamma_v(0)=v$ is defined up to time one, and the [exponential map](../../../../../exponential-map-riemannian-geometry.md) is $\exp_p(v)=\gamma_v(1)$.

The geodesic equation is invariant under affine rescaling of the parameter. Uniqueness therefore gives $\gamma_v(t)=\exp_p(tv)$ whenever these expressions are defined. In particular

$$
(d\exp_p)_0(w)=\left.\frac{d}{dt}\right|_0\exp_p(tw)
=\dot\gamma_w(0)=w.
$$

The [inverse function theorem](../../../../../inverse-function-theorem.md) now makes $\exp_p$ a diffeomorphism from a sufficiently small ball about zero in $T_pM$ onto a neighborhood of $p$. Choose a $g_p$-orthonormal basis $(e_i)$ and define coordinates by

$$
q=\exp_p\left(\sum_i x^i(q)e_i\right).
$$

These are [geodesic coordinates](../../../../../normal-coordinates.md), also called [normal coordinates](../../../../../normal-coordinates.md). They exist near every point. Radial coordinate rays $x^i(t)=tv^i$ are affinely parametrized geodesics issuing from $p$, and $g_{ij}(p)=\delta_{ij}$. Substitution of all such rays into the geodesic equation at $t=0$ gives $\Gamma^i{}_{jk}(p)v^jv^k=0$ for all $v$. Since the connection is torsion-free, these coefficients are symmetric in $j,k$; polarization gives $\Gamma^i{}_{jk}(p)=0$. Metric compatibility then gives $\partial_kg_{ij}(p)=0$. These statements concern the center $p$; they do not make every translated coordinate line a geodesic.

The precise [Gauss lemma](../../../../../gauss-s-lemma-riemannian-geometry.md) is

$$
\boxed{g_{\exp_p(v)}\big((d\exp_p)_v v,(d\exp_p)_v w\big)=g_p(v,w)}
$$

for $v$ in such a sufficiently small neighborhood and every $w\in T_pM$. Thus the exponential map preserves the radial pairing; in particular it takes the radial direction orthogonally to the tangent directions of spheres about zero.

To prove it, form the smooth [geodesic variation](../../../../../geodesic-variation.md)

$$
F(t,s)=\exp_p\big(t(v+sw)\big),\qquad
T=\partial_tF,\quad S=\partial_sF.
$$

All the curves with $s$ fixed are geodesics, so $D_tT=0$. The torsion-free [Levi-Civita connection](../../../../../levi-civita-connection.md) gives $D_tS=D_sT$ for this two-parameter map. This equality follows also by writing both derivatives in coordinates: the mixed partial derivatives agree and the Christoffel coefficients are symmetric. Metric compatibility yields

$$
\partial_t g(T,S)=g(T,D_tS)=g(T,D_sT)
=\tfrac12\partial_s g(T,T).
$$

The constant-speed property permitted in the question gives $g(T,T)=g_p(v+sw,v+sw)$ for every $t$. Thus at $s=0$ the last expression is $g_p(v,w)$. Since $F(0,s)=p$, we have $S(0,s)=0$, and integrating in $t$ gives $g(T,S)(t,0)=t\,g_p(v,w)$. At $t=1$, the two variation derivatives are $T(1,0)=(d\exp_p)_v v$ and $S(1,0)=(d\exp_p)_v w$, proving the lemma. Its radial-length assertion follows by taking $w=v$, and its orthogonality assertion by taking $w\perp v$. Only constant speed is used here; the PDF correctly states constancy of the length of the velocity vector, whose dot is lost in the TeX aid.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 14](../../paper-14-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

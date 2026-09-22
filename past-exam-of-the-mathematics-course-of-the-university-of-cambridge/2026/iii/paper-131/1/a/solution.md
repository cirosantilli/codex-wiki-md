<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a [connected](../../../../../../connected-space.md) [Riemannian manifold](../../../../../../riemannian-manifold.md) $(M,g)$, its [Riemannian distance](../../../../../../riemannian-distance.md) is

$$
d_g(p,q)=\inf_\gamma L_g(\gamma),
\qquad
L_g(\gamma)=\int_a^b|\dot\gamma(t)|_g\,dt,
$$

where the [infimum](../../../../../../infimum.md) is over the piecewise smooth curves from $p$ to $q$. Connectedness of a [smooth manifold](../../../../../../smooth-manifold.md) implies path connectedness, so this set of curves is nonempty.

The [Gauss lemma](../../../../../../gauss-s-lemma-riemannian-geometry.md) says that the differential of $\exp_p$ preserves the radial inner product: for $v,w\in T_pM$,

$$
g_{\exp_p(v)}\bigl((d\exp_p)_v v,(d\exp_p)_v w\bigr)=g_p(v,w).
$$

Consequently radial [geodesics](../../../../../../geodesic.md) from $p$ are orthogonal to the images of tangent vectors to spheres centred at the origin in $T_pM$. In a sufficiently small [normal neighbourhood](../../../../../../normal-neighbourhood.md) of $p$, this implies

$$
d_g(p,\exp_p v)=|v|_g:
$$

every competing curve has length at least the total variation of its radial coordinate, and the radial geodesic has that length.

The axioms $d_g(p,q)\geq0$, symmetry, and the [triangle inequality](../../../../../../triangle-inequality.md) follow directly from length and concatenation. Certainly $d_g(p,p)=0$. If $q\ne p$, choose a normal ball $B_g(p,r)$ that does not contain $q$. Every curve from $p$ to $q$ first meets its boundary, and its initial part has length at least $r$ by the Gauss lemma. Hence $d_g(p,q)\geq r>0$. Thus $d_g(p,q)=0$ if and only if $p=q$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 131](../../../paper-131-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

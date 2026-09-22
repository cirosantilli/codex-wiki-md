<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Work on a connected, finite-dimensional [Riemannian manifold](../../../../../riemannian-manifold.md) without boundary. It is [geodesically complete](../../../../../geodesic-completeness.md) if every maximal affinely parametrized [geodesic](../../../../../geodesic.md) has parameter domain $\mathbb R$. Equivalently, for every $p$ the [Riemannian exponential map](../../../../../exponential-map-riemannian-geometry.md) $\exp_p$ is defined on all of $T_pM$: any finite affine time can be rescaled to time one, and negative times correspond to reversing the initial velocity.

The [Hopf-Rinow lemma](../../../../../hopf-rinow-lemma.md) in its minimizing-geodesic form says: **if $\exp_p$ is defined on all of $T_pM$ for one point $p$, then every $q$ can be joined to $p$ by a geodesic of length $d(p,q)$.** We first establish the local ingredient, the [distance splitting through a small geodesic sphere](../../../../../distance-splitting-through-a-small-geodesic-sphere.md). If $D=d(p,q)>0$, choose $0<\varepsilon<D$ sufficiently small that the closed normal ball about $p$ is compact and radial lengths give [Riemannian distance](../../../../../riemannian-distance.md), as proved using the [Gauss lemma](../../../../../gauss-s-lemma-riemannian-geometry.md). Take paths from $p$ to $q$ of lengths tending to $D$. Their first intersections $x_j$ with its boundary sphere have a subsequence converging to some $x$ on the sphere. Their lengths are at least $\varepsilon+d(x_j,q)$, giving $D\geq\varepsilon+d(x,q)$. The [triangle inequality](../../../../../triangle-inequality.md) gives the reverse inequality. Therefore

$$
\boxed{d(p,q)=\varepsilon+d(x,q),\qquad d(p,x)=\varepsilon.}
$$

This splitting uses only a compact local [geodesic sphere](../../../../../geodesic-sphere.md), not completeness or the existence of a globally minimizing path.

We also need that [a minimizing broken geodesic has no corner](../../../../../a-minimizing-broken-geodesic-has-no-corner.md). To see this directly, let the incoming and outgoing unit tangents at a junction be $u$ and $v$. Choose one nearby point on each segment so that they and the junction lie in a common [convex normal neighbourhood](../../../../../convex-normal-neighbourhood.md). Move the junction with velocity $z$, joining it to those two fixed points by the unique short [geodesics](../../../../../geodesic.md). The [Gauss lemma](../../../../../gauss-s-lemma-riemannian-geometry.md), or the first variation formula, gives the derivative of the sum of their lengths as $\langle u-v,z\rangle$. If $u\ne v$, setting $z=v-u$ makes this derivative $-|u-v|^2<0$, contradicting minimality. Thus the tangent vectors agree, and uniqueness for the [geodesic equation](../../../../../geodesic-equation.md) makes the broken path one smooth [geodesic](../../../../../geodesic.md).

Now choose the unit-speed radial [geodesic](../../../../../geodesic.md) $\gamma$ through the point $x$ obtained by the distance splitting, with $\gamma(0)=p$ and $\gamma(\varepsilon)=x$. By the hypothesis on $\exp_p$, it is defined at least up to time $D$. Define

$$
A=\{t\in[\varepsilon,D]:d(\gamma(t),q)=D-t\}.
$$

This is a nonempty closed set. If $t\in A$, the [triangle inequality](../../../../../triangle-inequality.md) and the length of $\gamma|_{[0,t]}$ give

$$
D\leq d(p,\gamma(t))+d(\gamma(t),q)\leq t+(D-t)=D,
$$

so $d(p,\gamma(t))=t$: that geodesic segment minimizes. Let $t_* =\max A$. If $t_*<D$, apply the [distance splitting through a small geodesic sphere](../../../../../distance-splitting-through-a-small-geodesic-sphere.md) at $\gamma(t_*)$ with radius $0<\delta<D-t_*$. There is a point $y$, joined to $\gamma(t_*)$ by a short minimizing radial [geodesic](../../../../../geodesic.md) $\sigma$, for which

$$
d(\gamma(t_*),q)=\delta+d(y,q).
$$

The broken path $\gamma|_{[0,t_*]}*\sigma$ has length $t_*+\delta$. Moreover,

$$
D\leq d(p,y)+d(y,q)\leq t_*+\delta+d(y,q)=D.
$$

Consequently that broken path minimizes. It has no corner, so $\sigma$ is the continuation of $\gamma$ and $y=\gamma(t_*+\delta)$. The last distance equality puts $t_*+\delta$ in $A$, a contradiction. Hence $D\in A$ and $\gamma(D)=q$. This proves the [Hopf-Rinow lemma](../../../../../hopf-rinow-lemma.md), with the case $p=q$ supplied by the constant [geodesic](../../../../../geodesic.md).

The [Hopf-Rinow theorem](../../../../../hopf-rinow-theorem.md) asserts the equivalence of

- completeness for the [Riemannian distance](../../../../../riemannian-distance.md);
- [geodesic completeness](../../../../../geodesic-completeness.md);
- compactness of every closed bounded subset.

These conditions imply the existence of a [minimizing geodesic](../../../../../minimizing-geodesic.md) between any two points. Here is the deduction, including the implication back to geodesic completeness. If the manifold is [geodesically complete](../../../../../geodesic-completeness.md), the [Hopf-Rinow lemma](../../../../../hopf-rinow-lemma.md) applies at each point. For every $R\geq0$,

$$
\overline B(p,R)=\exp_p\bigl(\{v\in T_pM:|v|\leq R\}\bigr).
$$

One inclusion follows from the length of the radial [geodesic](../../../../../geodesic.md); the other follows by taking an initial velocity of a minimizing one. The tangent-space ball is compact, so the metric ball is compact as its continuous image. Every closed bounded set is a closed subset of such a ball and is compact. A [Cauchy sequence](../../../../../cauchy-sequence.md) is bounded and therefore has a convergent subsequence in a compact ball; the Cauchy property makes the whole sequence converge. This proves completeness of the [Riemannian distance](../../../../../riemannian-distance.md).

Conversely, assume metric completeness and let $\gamma:[0,b)\to M$ be a [geodesic](../../../../../geodesic.md) with $b<\infty$. Its speed $c$ is constant, so $d(\gamma(s),\gamma(t))\leq c|s-t|$. Completeness therefore gives a limit $q$ as $t\uparrow b$. Eventually $\gamma$ lies in a coordinate neighbourhood with compact closure on which the [Riemannian metric](../../../../../riemannian-metric.md) is uniformly comparable to the Euclidean metric. Its coordinate velocity is bounded by the constant-speed estimate. The [Christoffel symbols](../../../../../christoffel-symbol.md) are bounded there, so the [geodesic equation](../../../../../geodesic-equation.md)

$$
\ddot x^k=-\Gamma^k_{ij}(x)\dot x^i\dot x^j
$$

makes its coordinate acceleration bounded. Thus the coordinate velocity also has a limit $v$ at time $b$. The local existence and uniqueness theorem for smooth [ordinary differential equations](../../../../../ordinary-differential-equation.md) extends the solution from initial data $(q,v)$ past $b$, contradicting maximality. Reversing time treats a finite left endpoint. Hence metric completeness implies [geodesic completeness](../../../../../geodesic-completeness.md), and the preceding argument supplies compactness of closed bounded sets. Compactness of closed bounded sets already implies metric completeness by the Cauchy-sequence argument, completing all equivalences.

In fact, the one-point hypothesis of the [Hopf-Rinow lemma](../../../../../hopf-rinow-lemma.md) suffices for the theorem: the same closed-ball image argument at that point puts every Cauchy sequence in a compact ball, giving metric completeness and then geodesic completeness at every point. By contrast, the existence of a [minimizing geodesic](../../../../../minimizing-geodesic.md) for every pair alone does not imply completeness: an open Euclidean ball has minimizing straight segments between all its points but has Cauchy sequences converging to its missing boundary.

**Geodesic completeness, metric completeness and compactness of closed bounded sets are equivalent; under these conditions every pair is joined by a minimizing geodesic.**

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 12](../../paper-12-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

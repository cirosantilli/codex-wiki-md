<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Write $\widehat X=X_{/Y}$. The [formal completion of a scheme](../../../../../formal-completion-of-a-scheme.md) restricts on each chart to

$$
\widehat U_i=\operatorname{Spf}A_i,\qquad
A_i=\varprojlim_{n\geq0}\mathbb Z[x_i,y_i]/((x_i y_i)^{n+1}),
\qquad q=x_i y_i.
$$

Thus $\widehat X$ is a [formal scheme](../../../../../formal-scheme.md) over $\operatorname{Spf}\mathbb Z[[q]]$. The ordinary torus $D(q)$ has disappeared from its underlying space: every point of $\widehat X$ lies on $Y$. In particular, only adjacent completed charts intersect, and their two possible branch overlaps inside any one chart are disjoint.

Construct the action using the integral lattice [automorphism](../../../../../automorphism.md)

$$
S:N\longrightarrow N,\qquad S(a,b)=(a+3b,b).
$$

It carries $v_i$ to $v_{i+3}$ and $\sigma_i$ to $\sigma_{i+3}$, so induces a [toric morphism](../../../../../toric-morphism.md) $g:X\to X$ that is an [automorphism](../../../../../automorphism.md). It preserves the lattice projection to the second coordinate, hence preserves $q$ and $Y$. On the dense [algebraic torus](../../../../../algebraic-torus.md) it is

$$
(t,q)\longmapsto(q^3t,q).
$$

In the local coordinates this sends $U_i$ to $U_{i+3}$ with

$$
g^*(x_{i+3})=x_i,\qquad g^*(y_{i+3})=y_i.
$$

These identities show regularity on every chart without requiring $q$ to be invertible there. They also make the action continuous in the $q$-adic topology, so it extends to $\widehat X$. Its powers shift $D_i$ to $D_{i+3k}$; no nonzero power is the identity or fixes a point of the formal support. Therefore $G=\langle g\rangle\cong\mathbb Z$ is a nontrivial [infinite cyclic group](../../../../../infinite-cyclic-group.md) acting freely.

Construct the quotient explicitly, using three representative charts

$$
\mathfrak V_i=\operatorname{Spf}\left(\varprojlim_n
\mathbb Z[X_i,Y_i]/((X_iY_i)^{n+1})\right),\qquad i=0,1,2,
$$

with $q=X_iY_i$. Glue their branch opens cyclically, taking subscripts modulo three, by

$$
\boxed{D(Y_i)\subset\mathfrak V_i\ \cong\ D(X_{i+1})\subset\mathfrak V_{i+1},
\qquad X_{i+1}=Y_i^{-1},\quad Y_{i+1}=X_iY_i^2.}
$$

These are genuine [isomorphisms](../../../../../isomorphism.md) of [formal schemes](../../../../../formal-scheme.md). For example, the [completed localization of an adic ring](../../../../../completed-localization-of-an-adic-ring.md) on the first open is

$$
\Gamma(D(Y_i),\mathcal O)=\mathbb Z[Y_i,Y_i^{-1}][[q]],
$$

where $X_i=q/Y_i$. On the second it is $\mathbb Z[X_{i+1},X_{i+1}^{-1}][[q]]$, and the gluing sends $X_{i+1}$ to $Y_i^{-1}$ and $Y_{i+1}$ to $qY_i$. Thus it preserves $q$ and is continuous, with a continuous inverse.

Inside $\mathfrak V_i$ we have

$$
D(X_i)\cap D(Y_i)=D(q)=\varnothing.
$$

Consequently there are no triple-overlap conditions left to check: the two branch identifications in a chart have disjoint domains. By [gluing of schemes along open subschemes](../../../../../gluing-of-schemes-along-open-subschemes.md) in its formal version, the three charts produce a [formal scheme](../../../../../formal-scheme.md) $\mathfrak C$ over $\operatorname{Spf}\mathbb Z[[q]]$. Equivalently, reduce the same gluing modulo $q^{n+1}$ for every $n$; this constructs compatible [schemes](../../../../../scheme.md) $C_n$, all on the same underlying space, with $C_n=C_{n+1}\times\operatorname{Spec}\mathbb Z[q]/(q^{n+1})$. Their inverse system has precisely the displayed formal charts.

For every integer $i$, map $\widehat U_i$ isomorphically to $\mathfrak V_{\bar i}$ by identifying its coordinates with the corresponding capital-letter coordinates. The adjacent-chart formulas agree with the cyclic identifications, so these maps glue to

$$
\pi:\widehat X\longrightarrow\mathfrak C.
$$

They are invariant under $g$, and $\pi^{-1}(\mathfrak V_i)$ is the disjoint union of the translated opens $\widehat U_{i+3k}$, each mapping isomorphically onto $\mathfrak V_i$. The group permutes these copies transitively. Thus the fibres of $\pi$ are exactly the $G$-orbits, and invariant sections on this inverse image are exactly the sections on $\mathfrak V_i$.

To verify the quotient property also for morphisms, take a $G$-invariant morphism $h:\widehat X\to\mathfrak T$. Its restrictions to $\widehat U_0,\widehat U_1,\widehat U_2$ agree on the adjacent branch opens. On the closing overlap they agree because the translated chart $\widehat U_3$ has the same restriction as $\widehat U_0$ under $g$. Hence they descend to a unique morphism $\mathfrak C\to\mathfrak T$. This proves that the gluing is the [cyclic formal quotient of the infinite toric chain](../../../../../cyclic-formal-quotient-of-the-infinite-toric-chain.md):

$$
\boxed{\mathfrak C\cong X_{/Y}/\langle g\rangle,
\qquad g:(t,q)\mapsto(q^3t,q).}
$$

Its fibre modulo $q$ is a triangle of three [projective lines](../../../../../projective-line.md) over $\mathbb Z$, each meeting its two neighbours at its two boundary sections. More generally, a shift by any $m\geq3$ gives an $m$-gon. Completion is important here: translates of a formal chart are disjoint, whereas all ordinary toric charts still share the generic torus.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 17](../../paper-17-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Realize the [pullback vector bundle](../../../../../../pullback-vector-bundle.md) as

$$
\phi^*E=\{(p,v)\in M'\times E:\phi(p)=\pi(v)\},\qquad
\pi'(p,v)=p.
$$

Its fibre over $p$ is canonically $E_{\phi(p)}$, with the same [vector space](../../../../../../vector-space-split.md) operations. If a [vector bundle trivialization](../../../../../../vector-bundle-trivialization.md) over $U\subset M$ is $\tau_U(v)=(\pi(v),\widehat v)$, give the [pullback vector bundle](../../../../../../pullback-vector-bundle.md) the local trivialization

$$
T_U:(\pi')^{-1}(\phi^{-1}U)\longrightarrow\phi^{-1}U\times\mathbb R^r,
\qquad T_U(p,v)=(p,\widehat v).
$$

Declare these maps to be local homeomorphisms and use [coordinate charts](../../../../../../manifold-chart.md) on $M'$ to obtain a [smooth atlas](../../../../../../smooth-atlas.md) on the total space. On overlaps the [smooth transition maps](../../../../../../smooth-transition-map.md) are $(p,w)\mapsto(p,h(\phi(p))w)$, hence smooth and fibrewise linear. They satisfy the same cocycle identities as the original transition maps. This gives a well-defined smooth [vector bundle](../../../../../../vector-bundle.md), with smooth projection and rank $r$. It also gives the [subspace topology](../../../../../../subspace-topology.md) inherited from $M'\times E$: inside each product $\phi^{-1}(U)\times\pi^{-1}(U)$ the defining condition is the graph of $\phi$ in the base coordinates. Thus the total space is Hausdorff and second countable, as required for a [smooth manifold](../../../../../../smooth-manifold.md).

For a smooth [section of a vector bundle](../../../../../../section-of-a-vector-bundle.md) $s$ over $U$, its pulled-back section is more precisely $p\mapsto(p,s(\phi(p)))$. If $s$ has component column $u:U\to\mathbb R^r$ in the original [vector bundle trivialization](../../../../../../vector-bundle-trivialization.md), its component column in $T_U$ is $u\circ\phi$, which is smooth. **The pullback is a smooth rank-$r$ vector bundle, and every local section pulls back smoothly.**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 15](../../../paper-15-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The fibers must retain their base labels. In particular, a literal untagged union of fibers in $E$ is not sufficient when $f$ is not [injective](../../../../../../injective-function.md). Use the [pullback vector bundle](../../../../../../pullback-vector-bundle.md)

$$
f^*E=\{(p,e)\in N\times E:f(p)=\pi(e)\},\qquad \pi_f(p,e)=p.
$$

This makes precise the indexed-union notation in the PDF. For a [vector bundle trivialization](../../../../../../vector-bundle-trivialization.md) $\Phi_U(e)=(\pi(e),v)$, define

$$
\Psi_U:\pi_f^{-1}(f^{-1}U)\longrightarrow f^{-1}U\times\mathbb R^r,
\qquad(p,e)\longmapsto(p,v).
$$

It is a fiberwise [linear isomorphism](../../../../../../linear-isomorphism.md), with inverse $(p,v)\mapsto(p,\Phi_U^{-1}(f(p),v))$. The transition functions are $g_{VU}\circ f$, hence smooth. They satisfy the same cocycle identities as those of $E$ and give a smooth total space of [manifold dimension](../../../../../../dimension-of-a-manifold.md) $\dim N+r$.

One may also see that this is an [embedded submanifold](../../../../../../embedded-submanifold.md) of $N\times E$: in a bundle chart the constraint is the graph of the smooth map $f$ in the base coordinates, leaving the $r$ fiber coordinates free. Thus the chart construction agrees with its natural subspace smooth structure. No immersion or surjectivity hypothesis on $f$ is required. Therefore

$$
\boxed{f^*E\longrightarrow N\text{ is a rank-}r\text{ vector bundle}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 115](../../../paper-115-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

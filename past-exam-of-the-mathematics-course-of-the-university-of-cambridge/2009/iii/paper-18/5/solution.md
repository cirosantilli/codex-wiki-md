<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Fix a point $[L]\in\operatorname{Pic}^d(C)$ and put $V=H^0(C,L)$. The set of effective [Cartier divisors](../../../../../cartier-divisor-split.md) in its [divisor class](../../../../../divisor-class.md) is the [complete linear system of a divisor](../../../../../complete-linear-system-of-a-divisor.md), but identifying points alone would not prove the requested scheme assertion. We identify its functor on arbitrary parameter [schemes](../../../../../scheme.md), including nonreduced ones.

Let $T$ be a $k$-scheme and let $\mathcal D\subset C\times T$ be a relative effective degree-$d$ [Cartier divisor](../../../../../cartier-divisor-split.md) whose [Abel map of an algebraic curve](../../../../../abel-map-of-an-algebraic-curve.md) is the constant morphism $[L]$. The definition of the [Picard functor of a curve](../../../../../picard-functor-of-a-curve.md) says

$$
\mathcal O(\mathcal D)\cong\operatorname{pr}_C^*L\otimes\pi^*M
$$

for a [line bundle](../../../../../line-bundle.md) $M$ on $T$. Its canonical section is nonzero on every geometric fibre. Since the constant family has direct image $V\otimes_k\mathcal O_T$, this section determines a line subbundle

$$
M^{-1}\hookrightarrow V\otimes_k\mathcal O_T.
$$

It is a subbundle, rather than merely an injective sheaf map: locally some coordinate is nonzero on each residue field, hence a unit on a neighbourhood, so the quotient is locally free. Such a subbundle is exactly a $T$-point of the [projective space](../../../../../projective-space-split.md) $\mathbb P_{\mathrm{lines}}(V)$.

Conversely, its tautological line subbundle evaluates to a section of $\operatorname{pr}_C^*L\otimes\pi^*M$, nonzero on every geometric fibre. On the smooth integral fibres its zero locus is an effective [Cartier divisor](../../../../../cartier-divisor-split.md). The fibrewise regularity criterion gives a relative [Cartier divisor](../../../../../cartier-divisor-split.md) flat over $T$, of degree $d$, and its Picard class is constant $[L]$. These constructions are inverse and commute with arbitrary [base change](../../../../../base-change-of-a-morphism-of-schemes.md). Thus they identify functors, and therefore the scheme fibre itself:

$$
\boxed{a_d^{-1}([L])\cong\mathbb P_{\mathrm{lines}}(H^0(C,L))\cong\mathbb P^{h^0(C,L)-1}_k.}
$$

If $h^0(C,L)=0$, the fibre is empty, which is smooth as well. The argument remains valid over a point's residue field, so every scheme fibre, not just each closed geometric fibre, is smooth. Fibre dimensions can jump when $h^0(C,L)$ jumps; this does not assert that the entire [Abel map of an algebraic curve](../../../../../abel-map-of-an-algebraic-curve.md) is a [smooth morphism](../../../../../smooth-morphism.md).

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 18](../../paper-18-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

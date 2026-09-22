<h1 id="5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For a [smooth projective curve](../../../../../../smooth-projective-curve.md) $C$, let $g=h^1(C,\mathcal O_C)$ be its [geometric genus](../../../../../../geometric-genus.md), let $K_C$ be a [canonical divisor](../../../../../../canonical-divisor.md), and write $\ell(D)=h^0(C,\mathcal O_C(D))$ for the [dimension of a vector space](../../../../../../dimension-vector-space.md) of the [Riemann-Roch space](../../../../../../riemann-roch-space.md). The [Riemann-Roch theorem](../../../../../../riemann-roch-theorem.md) says

$$
\boxed{\ell(D)-\ell(K_C-D)=\deg D+1-g}
$$

for every [divisor on an algebraic curve](../../../../../../divisor-on-an-algebraic-curve.md) $D$ on $C$.

Here is the [cohomological proof of Riemann-Roch for curves](../../../../../../cohomological-proof-of-riemann-roch-for-curves.md). At a [closed point](../../../../../../closed-point.md) $P$, the [local ring](../../../../../../local-ring.md) is a [discrete valuation ring](../../../../../../discrete-valuation-ring.md). A local uniformizer shows that increasing the allowed pole order by one gives the [short exact sequence](../../../../../../short-exact-sequence.md) of [sheaves](../../../../../../sheaf-mathematics.md)

$$
0\longrightarrow\mathcal O_C(D-P)\longrightarrow\mathcal O_C(D)
\longrightarrow k(P)\longrightarrow0.
$$

The last term is a length-one [skyscraper sheaf](../../../../../../skyscraper-sheaf.md); its precise identification with $k$ is noncanonical, but its [sheaf cohomology](../../../../../../sheaf-cohomology.md) has $h^0=1$ and $h^1=0$. All the relevant groups of [sheaf cohomology](../../../../../../sheaf-cohomology.md) are finite-dimensional because $C$ is a [projective variety](../../../../../../projective-variety.md), and coherent [sheaf cohomology](../../../../../../sheaf-cohomology.md) above degree one vanishes on a [algebraic curve](../../../../../../algebraic-curve.md). The [long exact sequence in sheaf cohomology](../../../../../../long-exact-sequence-in-sheaf-cohomology.md) therefore gives

$$
\chi(\mathcal O_C(D))=\chi(\mathcal O_C(D-P))+1,
\qquad \chi(\mathcal F)=h^0(C,\mathcal F)-h^1(C,\mathcal F).
$$

Since $k$ is an [algebraically closed field](../../../../../../algebraically-closed-field.md), every [closed point](../../../../../../closed-point.md) has degree one. Iterating this identity for both positive and negative coefficients of $D$ proves

$$
\chi(\mathcal O_C(D))=\deg D+\chi(\mathcal O_C).
$$

Every [global regular function](../../../../../../global-regular-function.md) on a [projective variety](../../../../../../projective-variety.md) which is an [irreducible variety](../../../../../../irreducible-variety.md) is constant; hence $h^0(C,\mathcal O_C)=1$ and $\chi(\mathcal O_C)=1-g$.

Finally apply [Serre duality](../../../../../../serre-duality.md) for a [smooth projective curve](../../../../../../smooth-projective-curve.md):

$$
H^1(C,\mathcal O_C(D))^*
\cong H^0(C,\omega_C\otimes\mathcal O_C(-D))
=H^0(C,\mathcal O_C(K_C-D)).
$$

Taking [dimensions of a vector space](../../../../../../dimension-vector-space.md) and inserting this in the [Euler characteristic of a coherent sheaf](../../../../../../euler-characteristic-of-a-coherent-sheaf.md) identity proves the displayed [Riemann-Roch theorem](../../../../../../riemann-roch-theorem.md). The substantial inputs from [sheaf cohomology](../../../../../../sheaf-cohomology.md) are finiteness and vanishing for coherent [sheaves](../../../../../../sheaf-mathematics.md) on a [projective curve](../../../../../../projective-curve.md), and [Serre duality](../../../../../../serre-duality.md); the change of [Euler characteristic of a coherent sheaf](../../../../../../euler-characteristic-of-a-coherent-sheaf.md) is proved directly by the point exact sequence. In particular the argument handles negative as well as effective [divisors on an algebraic curve](../../../../../../divisor-on-an-algebraic-curve.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [5](../../5.md)
3. [Paper 13](../../../paper-13-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

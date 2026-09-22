<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Use the finite map $f:C\to\mathbb P^1$ from the preceding solution. The inverse images of the two standard affine charts and of their intersection are affine, because $f$ is finite. The [vanishing of quasi-coherent cohomology on an affine scheme](../../../../../vanishing-of-quasi-coherent-cohomology-on-an-affine-scheme.md) therefore lets their two-term [Čech cochain complex](../../../../../cech-cochain-complex.md) compute $H^i(C,E)$. It has terms only in degrees zero and one, proving

$$
\boxed{H^i(C,E)=0\qquad(i\geq2).}
$$

This actually applies to every [quasi-coherent sheaf](../../../../../quasi-coherent-sheaf.md) on $C$.

For a [smooth projective curve](../../../../../smooth-projective-curve.md) with $H^0(C,\mathcal O_C)=k$, define its [genus of a smooth projective curve](../../../../../genus-of-a-smooth-projective-curve.md) by

$$
\boxed{g=\dim_kH^1(C,\mathcal O_C).}
$$

The preceding [Serre duality](../../../../../serre-duality.md) also gives $g=\dim_kH^0(C,\Omega^1_C)$. The condition on constants holds in particular for a geometrically connected smooth projective curve. It makes $g$ equal to the [arithmetic genus](../../../../../arithmetic-genus.md) $1-\chi(\mathcal O_C)$. We state the theorem with this usual convention and then give the formula valid without that condition.

For a [divisor on an algebraic curve](../../../../../divisor-on-an-algebraic-curve.md) $D$ and a [canonical divisor](../../../../../canonical-divisor.md) $K$ with $\mathcal O(K)\cong\Omega^1_C$, the [Riemann-Roch theorem](../../../../../riemann-roch-theorem.md) is

$$
\boxed{\ell(D)-\ell(K-D)=\deg_kD+1-g,\qquad\ell(D)=h^0(C,\mathcal O(D)).}
$$

The degree over an arbitrary [field](../../../../../field.md) is weighted by residue degrees: $\deg_kD=\sum_pn_p[k(p):k]$ when $D=\sum_pn_pp$. Equivalently, for a [line bundle](../../../../../line-bundle.md) $L$,

$$
h^0(L)-h^0(\Omega^1_C\otimes L^{-1})=\deg_kL+1-g.
$$

We now prove it via [Riemann-Roch via elementary modifications](../../../../../riemann-roch-via-elementary-modifications.md).

For any closed point $p$ and any [line bundle](../../../../../line-bundle.md) $L$, the exact sequence

$$
0\longrightarrow L(-p)\longrightarrow L\longrightarrow L|_p\longrightarrow0
$$

has a [skyscraper sheaf](../../../../../skyscraper-sheaf.md) as its quotient, with $k$-dimension $[k(p):k]$. This follows locally from a uniformizer of the [discrete valuation ring](../../../../../discrete-valuation-ring.md) at $p$: a local line-bundle generator modulo that uniformizer spans one copy of $k(p)$. The quotient has zero higher cohomology, as it is the direct image from a finite affine scheme. The [long exact sequence in sheaf cohomology](../../../../../long-exact-sequence-in-sheaf-cohomology.md) and the proved higher vanishing give

$$
\chi(L)-\chi(L(-p))=[k(p):k],\qquad\chi(L)=h^0(L)-h^1(L).
$$

Every [line bundle](../../../../../line-bundle.md) has a nonzero [rational section of a line bundle](../../../../../rational-section-of-a-line-bundle.md), whose local orders give a [divisor on an algebraic curve](../../../../../divisor-on-an-algebraic-curve.md) $D$ with $L\cong\mathcal O(D)$. Iterating the displayed identity, adding or subtracting closed points with their multiplicities, gives

$$
\chi(\mathcal O(D))=\deg_kD+\chi(\mathcal O_C).
$$

For the constants convention above, $\chi(\mathcal O_C)=1-g$. The [dualizing sheaf on a smooth projective curve](../../../../../dualizing-sheaf-on-a-smooth-projective-curve.md) gives $h^1(\mathcal O(D))=h^0(\mathcal O(K-D))$, which converts this Euler-characteristic identity into the stated [Riemann-Roch theorem](../../../../../riemann-roch-theorem.md). This proves the formula over arbitrary $k$, without assuming the closed points are $k$-rational.

For [vector bundles](../../../../../vector-bundle.md), the corresponding formula is

$$
\boxed{\chi(E)=\deg_k(\det E)+\operatorname{rank}(E)(1-g).}
$$

To see it, saturate a rational rank-one subspace to a [line subbundle](../../../../../line-subbundle.md) and induct on rank. Both [Euler characteristic of a coherent sheaf](../../../../../euler-characteristic-of-a-coherent-sheaf.md) and the degree of the determinant are additive in the resulting short exact sequence. The line-bundle formula just proved starts the induction.

Taking $L=\Omega^1_C$ and using duality gives $h^0(\Omega^1_C)=g$, $h^1(\Omega^1_C)=1$, and hence $\deg_k\Omega^1_C=2g-2$. In particular a [line bundle](../../../../../line-bundle.md) of degree greater than $2g-2$ has zero first cohomology: its dual twisted by $\Omega^1_C$ has negative degree, and a negative-degree line bundle has no nonzero section, since any section would have an [effective divisor](../../../../../effective-cartier-divisor.md) of zeros.

If the term “curve over $k$” is used without requiring $H^0(\mathcal O_C)=k$, the unconditional formula we proved is

$$
\boxed{\chi(L)=\deg_kL+\chi(\mathcal O_C).}
$$

Writing $g=h^1(\mathcal O_C)$ then replaces $1-g$ by $h^0(\mathcal O_C)-g$. For example, $\mathbb P^1_{k'}$ viewed as a $k$-curve for a finite separable extension $k'/k$ has $h^0(\mathcal O_C)=[k':k]$, so a literal constant term $1$ would be incorrect. Alternatively the [arithmetic genus](../../../../../arithmetic-genus.md) $p_a=1-\chi(\mathcal O_C)$ gives the formula with constant $1-p_a$. The constants hypothesis for the usual genus is recorded in [Stacks Project, genus of a curve](https://stacks.math.columbia.edu/tag/0BY6).

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 23](../../paper-23-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

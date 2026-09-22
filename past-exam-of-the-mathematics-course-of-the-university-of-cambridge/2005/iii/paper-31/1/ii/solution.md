<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use arithmetic [Frobenius automorphisms](../../../../../../frobenius-automorphism.md): residues are raised to the size of the base [residue field](../../../../../../residue-field.md). Let $S$ contain the finite primes ramified in the finite [abelian extension](../../../../../../abelian-extension.md) $L/K$. The [Artin map](../../../../../../artin-reciprocity-law.md) is the [group homomorphism](../../../../../../group-homomorphism.md)

$$
\operatorname{Art}_{L/K}:I_K^S\longrightarrow\operatorname{Gal}(L/K),\qquad
\prod_{\mathfrak p\notin S}\mathfrak p^{n_{\mathfrak p}}
\longmapsto\prod_{\mathfrak p\notin S}\operatorname{Frob}_{\mathfrak p}^{n_{\mathfrak p}},
$$

where $I_K^S$ is the [group](../../../../../../group-split.md) of [fractional ideals](../../../../../../fractional-ideal.md) supported outside $S$. The [Artin symbol](../../../../../../artin-symbol.md) $\operatorname{Frob}_{\mathfrak p}$ is independent of the prime above $\mathfrak p$, since the extension is abelian. [Commutativity](../../../../../../commutativity.md) makes the displayed extension from [prime ideals](../../../../../../prime-ideal.md) well defined. Defining this map does not yet assert the [Artin reciprocity law](../../../../../../artin-reciprocity-law.md), which describes its congruence [group kernel](../../../../../../kernel-of-a-group-homomorphism.md).

For an intermediate [field](../../../../../../field.md) $K\subseteq E\subseteq L$, restriction gives

$$
\boxed{\operatorname{Art}_{L/K}(\mathfrak a)|_E=\operatorname{Art}_{E/K}(\mathfrak a).}
$$

To prove it, start with an unramified prime $\mathfrak p$ and a prime of $L$ above it. Its [Frobenius automorphism](../../../../../../frobenius-automorphism.md) acts on the residue of every [integral element](../../../../../../integral-element.md) of $E$ by raising it to $N\mathfrak p$. Its restriction is therefore the [Frobenius automorphism](../../../../../../frobenius-automorphism.md) for $E/K$ at the restricted prime. The identity for all allowed [fractional ideals](../../../../../../fractional-ideal.md) follows by the [group homomorphism](../../../../../../group-homomorphism.md) property. On [Galois groups](../../../../../../galois-group.md), restriction is the quotient by $\operatorname{Gal}(L/E)$, so passing to a subextension quotients the [Artin map](../../../../../../artin-reciprocity-law.md) accordingly.

Now let $E/K$ be any finite extension and put $M=LE$. This is the translated extension: $M/E$ is abelian, and restriction identifies $\operatorname{Gal}(M/E)$ with $\operatorname{Gal}(L/(L\cap E))$. A prime $\mathfrak q$ of $E$ above a prime $\mathfrak p\notin S$ is unramified in $M/E$, because forming a [compositum](../../../../../../field-compositum.md) with $E$ preserves an [unramified extension](../../../../../../unramified-extension.md). Put $r=f(\mathfrak q/\mathfrak p)$. The residue-field sizes satisfy $N\mathfrak q=(N\mathfrak p)^r$. Consequently the restriction to $L$ of Frobenius at $\mathfrak q$ acts on its integral residues by raising them to $(N\mathfrak p)^r$, giving

$$
\operatorname{Frob}_{\mathfrak q}(M/E)|_L
=\operatorname{Frob}_{\mathfrak p}(L/K)^r.
$$

But the [ideal norm](../../../../../../ideal-norm.md) is $N_{E/K}\mathfrak q=\mathfrak p^r$. Multiplying this prime-by-prime identity proves

$$
\boxed{\operatorname{Art}_{M/E}(\mathfrak a)|_L
=\operatorname{Art}_{L/K}(N_{E/K}\mathfrak a).}
$$

This is [restriction and norm compatibility of the Artin map](../../../../../../restriction-and-norm-compatibility-of-the-artin-map.md). The [fractional ideal](../../../../../../fractional-ideal.md) $\mathfrak a$ must be supported over primes unramified in $L/K$. No assumption that $E/K$ itself is unramified or Galois is needed. With geometric rather than [arithmetic Frobenius](../../../../../../frobenius-automorphism.md), both maps are inverted and the compatibility identities remain unchanged.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 31](../../../paper-31-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

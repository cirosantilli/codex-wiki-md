<h1 id="18h/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Choose $\alpha$ with $\alpha^n=a$. The roots of $x^n-a$ are $\alpha\zeta_n^j$, so $F=K(\alpha)$ contains every root. Conversely their ratios generate the roots of unity, so $F$ is precisely the [splitting field](../../../../../../splitting-field.md) of $x^n-a$ over $\mathbb Q$. In characteristic zero this polynomial is [separable polynomial](../../../../../../separable-polynomial.md), since $a\ne0$, and a splitting field of a separable polynomial is a [Galois extension](../../../../../../finite-galois-extension.md).

Each automorphism over $K$ sends $\alpha$ to $\alpha\zeta_n^j$. The map $\sigma\mapsto\sigma(\alpha)/\alpha$ embeds $\operatorname{Gal}(F/K)$ into the cyclic group $\mu_n$: it is multiplicative because the automorphisms fix roots of unity, and injective because $\alpha$ generates $F/K$. Hence this group is cyclic, of order dividing $n$.

For a Galois intermediate field $K/\mathbb Q$, restriction of automorphisms gives an exact sequence

$$
1\longrightarrow\operatorname{Gal}(F/K)\longrightarrow\operatorname{Gal}(F/\mathbb Q)\longrightarrow\operatorname{Gal}(K/\mathbb Q)\longrightarrow1.
$$

Surjectivity uses the extension theorem for embeddings into a normal splitting field. Both kernel and quotient are abelian, so the [commutator subgroup](../../../../../../commutator-subgroup.md) of $\operatorname{Gal}(F/\mathbb Q)$ lies in the abelian kernel. Its next commutator subgroup is trivial. Thus

$$
\boxed{\operatorname{Gal}(F/\mathbb Q)\text{ is soluble, with derived length at most two}.}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [18H](../../18h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

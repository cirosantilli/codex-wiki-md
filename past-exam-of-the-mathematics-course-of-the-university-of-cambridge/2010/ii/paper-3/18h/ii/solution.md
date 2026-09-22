<h1 id="18h/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $L=F(\mu_n)$. Its [Galois group](../../../../../../galois-group.md) embeds into $(\mathbb Z/n\mathbb Z)^\times$, by sending an automorphism to the exponent in its action on $\zeta_n$. It is therefore finite abelian, of order dividing $\varphi(n)$. The finite case of the [Fundamental theorem of finitely generated abelian groups](../../../../../../fundamental-theorem-of-finitely-generated-abelian-groups.md) supplies a subgroup chain whose successive quotients are cyclic of [prime](../../../../../../prime-number.md) order $\ell$. Every such $\ell<n$, since $\ell\le\varphi(n)<n$ for $n>1$ (and for $n=2$ the possible [prime](../../../../../../prime-number.md) is $2$, whose roots of unity already lie in every characteristic-zero field). Thus every intermediate base contains $\mu_\ell$, because $F$ contains all roots of unity of orders smaller than $n$.

Each cyclic degree-$\ell$ step $E'/E$ is a [Kummer extension](../../../../../../kummer-extension.md). Here is the relevant criterion explicitly. For a generator $\sigma$ and a primitive $\ell$th root $\zeta\in E$, the operator $\sum_{j=0}^{\ell-1}\zeta^{-j}\sigma^j$ is not identically zero, by linear independence of distinct [field automorphisms](../../../../../../field-automorphism.md). Choose its nonzero value $a$; then $\sigma(a)=\zeta a$, so $a^\ell\in E$ and $a\notin E$. Since the degree is [prime](../../../../../../prime-number.md), $E'=E(a)$ is obtained by adjoining an $\ell$th radical. Applying this to the subgroup chain proves **$F(\mu_n)/F$ is a succession of [Kummer extensions](../../../../../../kummer-extension.md)**.

Finally use strong induction on $n$, for arbitrary characteristic-zero base fields. Successively adjoining the roots $\zeta_1,\ldots,\zeta_{n-1}$ is contained in a Kummer tower by the induction hypothesis, applied over each current base. The just-proved assertion then adjoins $\zeta_n$ by further Kummer steps. Hence any cyclotomic extension is contained in a Kummer tower. In the given cyclotomic-and-Kummer tower for a soluble extension, replace every cyclotomic step by such a tower; enlarge subsequent steps by compositum with the new intermediate fields. Base change preserves radical adjunction and the requisite roots of unity, possibly making a step trivial. Thus **every finite soluble extension is contained in a succession of [Kummer extensions](../../../../../../kummer-extension.md)**.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [18H](../../18h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $G=\operatorname{Gal}(L/K)$. A [semilinear action](../../../../../semilinear-action.md) on an $L$-[vector space](../../../../../vector-space-split.md) $V$ is an additive action with $\sigma(av)=\sigma(a)\sigma(v)$. The [Galois descent of vector spaces](../../../../../galois-descent-of-vector-spaces.md) theorem says that $V^G$ is a $K$-[vector space](../../../../../vector-space-split.md) and the natural map

$$
L\otimes_KV^G\longrightarrow V,\qquad a\otimes v\longmapsto av
$$

is an isomorphism. In particular $\dim_KV^G=\dim_LV$. Morphisms also descend: an $L$-linear equivariant map is the scalar extension of its restriction to invariant subspaces.

We prove that the invariant vectors span $V$ over $L$, without dividing by $|G|$. For $a\in L$ and $v\in V$, the vector

$$
T_a(v)=\sum_{\sigma\in G}\sigma(a)\sigma(v)
$$

is invariant, because every $\tau\in G$ merely permutes the terms. Suppose their $L$-span were proper. There would be a nonzero $L$-[linear functional](../../../../../linear-functional.md) $\lambda$ annihilating that span. For each fixed $v$, we would have

$$
\sum_{\sigma\in G}\lambda(\sigma(v))\sigma(a)=0\qquad\text{for every }a\in L.
$$

The [Artin independence theorem](../../../../../linear-independence-of-distinct-field-embeddings.md) makes all coefficients zero, in particular $\lambda(v)=0$ for every $v$, a contradiction. To recall its elementary proof, take a nontrivial linear relation between distinct field automorphisms with the fewest nonzero coefficients. Replace the input $a$ by $ab$ and subtract one automorphism's value on $b$ times the original relation. Choose $b$ on which two participating automorphisms differ. The resulting nonzero relation has fewer terms, contradicting minimality.

Choose an $L$-basis $v_1,\ldots,v_m$ consisting of invariant vectors. If $v=\sum_i a_iv_i$ is invariant, uniqueness of coordinates gives $\sigma(a_i)=a_i$ for every $\sigma$, so every $a_i$ lies in $K$. These vectors are therefore a $K$-basis of $V^G$, proving the displayed map is an isomorphism. Restriction and scalar extension are visibly inverse on equivariant morphisms, completing the descent theorem. The argument remains valid when the characteristic divides $|G|$.

Now put $B=M_n(L)$, and let $\sigma_0$ act on $B$ by applying $\sigma$ to each entry. The group $\operatorname{Aut}_L(B)$ is a $G$-group under $\sigma(h)=\sigma_0h\sigma_0^{-1}$. Its [nonabelian first cohomology](../../../../../nonabelian-first-cohomology.md) consists of cocycles $c_\sigma$ satisfying

$$
c_{\sigma\tau}=c_\sigma\sigma(c_\tau),
$$

modulo $c'_\sigma=b c_\sigma\sigma(b)^{-1}$ for $b\in\operatorname{Aut}_L(B)$. This convention is equivalent to the usual one after replacing $b$ by its inverse. The matrix-automorphism calculation above identifies this coefficient group with $\operatorname{PGL}_n(L)$.

For a [central simple algebra](../../../../../central-simple-algebra.md) $A$ of degree $n$ split by $L$, choose $\phi:A\otimes_KL\to B$. Transport the natural [semilinear action](../../../../../semilinear-action.md) to $T_\sigma=\phi(1\otimes\sigma)\phi^{-1}$ and set

$$
c_\sigma=T_\sigma\sigma_0^{-1}.
$$

It is $L$-linear and multiplicative, and $T_\sigma T_\tau=T_{\sigma\tau}$ gives the cocycle identity. Replacing $\phi$ by $b\phi$ changes $c$ by the displayed coboundary equivalence. Isomorphic $K$-algebras give the same class, so this defines the [descent classification of central simple algebras](../../../../../descent-classification-of-central-simple-algebras.md) map naturally.

Conversely, a cocycle defines a semilinear algebra action $T_\sigma=c_\sigma\sigma_0$. Let

$$
A_c=B^{T(G)}.
$$

The vector-space descent theorem gives $A_c\otimes_KL\cong B$, with the natural map also respecting multiplication and the identity. Hence $\dim_KA_c=n^2$. If $I$ is a nonzero two-sided ideal of $A_c$, then $I\otimes_KL$ is a nonzero ideal of $B$, so it is all of $B$. Dimensions force $I=A_c$, proving simplicity. If $z$ is central in $A_c$, it commutes with its $L$-span $B$, and thus is a scalar matrix with scalar $a\in L$. Twisted invariance of a scalar matrix means $\sigma(a)=a$, so $a\in K$. The center is exactly $K$. Thus $A_c$ is central simple, of degree $n$, and split by $L$.

Equivalent cocycles have conjugate semilinear actions: $T'_\sigma=bT_\sigma b^{-1}$, so $b$ restricts to a $K$-algebra isomorphism between the fixed algebras. In the other direction, an isomorphism of fixed algebras extends to an $L$-algebra automorphism of $B$ and intertwines the two actions, giving exactly that equivalence relation. Starting from $A$ recovers the fixed algebra of $A\otimes L$, namely $A$; starting from a cocycle recovers its action. Therefore

$$
\boxed{\operatorname{CSA}_n(L/K)\ \cong\ H^1(G,\operatorname{Aut}_L(M_n(L)))\ =\ H^1(G,\operatorname{PGL}_n(L))}.
$$

This is a bijection of pointed sets, with the split algebra corresponding to the trivial cocycle. Fixed-degree algebra classes do not carry the [Brauer group](../../../../../brauer-group.md)'s tensor-product group law, so a pointed-set interpretation is the appropriate meaning of the isomorphism here.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 21](../../paper-21-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

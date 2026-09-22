<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

An [algebraic line bundle](../../../../../invertible-module.md) over $A$ is an [invertible module](../../../../../invertible-module.md): a [finitely generated projective module](../../../../../finite-projective-module.md) $L$ such that $L_{\mathfrak p}\cong A_{\mathfrak p}$ for every [prime ideal](../../../../../prime-ideal.md) $\mathfrak p$. Define the [Picard group of a ring](../../../../../picard-group-of-a-ring.md) as the set of its isomorphism classes, with

$$
[L][K]=[L\otimes_AK].
$$

The [tensor product of modules](../../../../../tensor-product-of-modules.md) of two finite [projective modules](../../../../../projective-module.md) is finite projective: write each as a direct summand of a finite [free module](../../../../../free-module.md) and tensor the two decompositions. Localization gives $(L\otimes_AK)_{\mathfrak p}\cong A_{\mathfrak p}$, so this multiplication stays within the set of [invertible modules](../../../../../invertible-module.md). It is well defined on isomorphism classes. The associativity and symmetry isomorphisms of the [tensor product](../../../../../tensor-product.md) give associativity and commutativity, and $[A]$ is the identity.

Let $L^*=\operatorname{Hom}_A(L,A)$ be the [dual module](../../../../../dual-module.md). A finite direct-summand presentation shows that $L^*$ is finite projective and that localization commutes with this dual. Since $L_{\mathfrak p}$ is free of rank one, so is $(L^*)_{\mathfrak p}$. The [evaluation homomorphism](../../../../../evaluation-homomorphism.md)

$$
L\otimes_AL^*\longrightarrow A,\qquad \ell\otimes\lambda\longmapsto\lambda(\ell)
$$

is an [isomorphism](../../../../../isomorphism.md) after every prime localization. Its kernel and cokernel are therefore zero, by [exactness of localization](../../../../../exactness-of-localization.md) and [localization detects zero elements](../../../../../localization-detects-zero-elements.md) for modules. Thus **$[L]^{-1}=[L^*]$**, proving that $\operatorname{Pic}(A)$ is an [abelian group](../../../../../abelian-group.md).

For a [ring homomorphism](../../../../../ring-homomorphism.md) $f:A\to B$, tensoring a split presentation $L\oplus L'\cong A^r$ gives $(B\otimes_AL)\oplus(B\otimes_AL')\cong B^r$, so $B\otimes_AL$ is finite projective. For $\mathfrak q\in\operatorname{Spec}B$ put $\mathfrak p=f^{-1}(\mathfrak q)$. Every element of $A\setminus\mathfrak p$ becomes a [unit](../../../../../unit-in-a-ring.md) in $B_{\mathfrak q}$, and

$$
(B\otimes_AL)_{\mathfrak q}\cong B_{\mathfrak q}\otimes_{A_{\mathfrak p}}L_{\mathfrak p}\cong B_{\mathfrak q}.
$$

This proves [base change of invertible modules](../../../../../base-change-of-invertible-modules.md). Moreover, the canonical map

$$
(B\otimes_AL)\otimes_B(B\otimes_AK)\longrightarrow B\otimes_A(L\otimes_AK),\qquad (b\otimes\ell)\otimes(b'\otimes k)\longmapsto bb'\otimes(\ell\otimes k)
$$

is an [isomorphism](../../../../../isomorphism.md), with inverse $b\otimes(\ell\otimes k)\mapsto(b\otimes\ell)\otimes(1\otimes k)$. It shows that $[L]\mapsto[B\otimes_AL]$ is a [group homomorphism](../../../../../group-homomorphism.md). Identity maps induce the identity, and for $A\to B\to C$, the associativity isomorphism $C\otimes_B(B\otimes_AL)\cong C\otimes_AL$ proves composition compatibility. Therefore **$\operatorname{Pic}$ is a covariant functor to abelian groups**.

The [polynomial ring](../../../../../polynomial-ring.md) $\mathbb C[x]$ is a [principal ideal domain](../../../../../principal-ideal-domain.md) by division with remainder. A submodule $N$ of a finite free module over a [principal ideal domain](../../../../../principal-ideal-domain.md) is free: induct on the ambient rank, project onto the first coordinate, and note that the image is a principal [ideal](../../../../../ideal.md), hence either zero or a free rank-one module. This gives a split exact sequence with that image as quotient; the kernel lies in a free module of one smaller rank, completing the induction. A finite [projective module](../../../../../projective-module.md) is such a submodule, and so is free. An [invertible module](../../../../../invertible-module.md) has rank one after passing to the [fraction field](../../../../../field-of-fractions.md), so its free rank is exactly one. Hence every [algebraic line bundle](../../../../../invertible-module.md) over $\mathbb C[x]$ is trivial and

$$
\boxed{\operatorname{Pic}(\mathbb C[x])=0.}
$$

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 3](../../paper-3-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

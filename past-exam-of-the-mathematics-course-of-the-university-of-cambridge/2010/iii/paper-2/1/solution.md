<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Write $A=kG$ and $J=J(A)$, its [Jacobson radical](../../../../../jacobson-radical.md). First suppose the [characteristic](../../../../../characteristic-of-a-field.md) is $p>0$. We prove the counting statement through the [cocenter of a finite-dimensional algebra](../../../../../cocenter-of-a-finite-dimensional-algebra.md)

$$
C(A)=A/[A,A],
$$

where $[A,A]$ is the linear span of commutators, not an ideal. In a [group algebra](../../../../../group-algebra.md), this span is exactly the span of differences of conjugate group elements: $gh-hg$ is such a difference, and $xgx^{-1}-g=[x,gx^{-1}]$. Consequently $C(A)$ has one [basis vector](../../../../../basis-vector.md) for each [conjugacy class](../../../../../conjugacy-class.md).

There is a well-defined [Frobenius map on an algebra cocenter](../../../../../frobenius-map-on-an-algebra-cocenter.md)

$$
F:C(A)\longrightarrow C(A),\qquad [a]\longmapsto[a^p].
$$

Here $F$ is additive and $F(c[a])=c^pF([a])$. To prove additivity, expand $(a+b)^p$ into words of length $p$. Cyclic rotations of a word are equal modulo commutators. Every nonconstant word has a rotation orbit of length $p$, so its orbit contributes zero; only $a^p,b^p$ remain. Also

$$
[(xy-yx)^p]=[(xy)^p]-[(yx)^p]=0,
$$

because the two products are cyclic rotations. Additivity then shows that the whole commutator subspace maps to zero, proving well-definedness on the quotient.

Let $s$ be the number of [simple modules](../../../../../irreducible-module.md) up to isomorphism. The [semisimple algebra](../../../../../semisimple-algebra.md) $A/J$ is $\prod_{\nu=1}^sM_{d_\nu}(k)$: over an [algebraically closed field](../../../../../algebraically-closed-field.md), a finite-dimensional [division algebra](../../../../../division-algebra.md) is the [field](../../../../../field.md) itself, since the [minimal polynomial](../../../../../minimal-polynomial.md) of any element splits into linear factors and a [division algebra](../../../../../division-algebra.md) has no zero divisors. In a [matrix algebra](../../../../../matrix-algebra.md), the commutator subspace is precisely the [traceless matrices](../../../../../traceless-matrix.md). Off-diagonal [matrix units](../../../../../matrix-unit.md) are commutators, and $E_{ii}-E_{jj}=[E_{ij},E_{ji}]$; these span that subspace in every characteristic. Thus

$$
C(A/J)\cong k^s.
$$

The map induced by $F$ on each coordinate is $z\mapsto z^p$, since $\operatorname{tr}(B^p)=(\operatorname{tr}B)^p$. This is bijective because $k$ is a [perfect field](../../../../../perfect-field.md).

The natural surjection $C(A)\twoheadrightarrow C(A/J)$ has [kernel](../../../../../kernel-of-a-linear-map.md) $(J+[A,A])/[A,A]$. Every [kernel](../../../../../kernel-of-a-linear-map.md) class has a representative in $J$. Since $J$ is nilpotent, $F^N$ kills that [kernel](../../../../../kernel-of-a-linear-map.md) for sufficiently large $N$. On the quotient it remains bijective, so its image has dimension exactly $s$. On the conjugacy-class basis, however,

$$
F^N([g])=[g^{p^N}].
$$

For large $N$, every $g^{p^N}$ is a [p-regular element](../../../../../p-regular-element.md); moreover the $p^N$-power map permutes the p-regular conjugacy classes, because an inverse exponent can be chosen modulo the prime-to-$p$ part of the exponent of $G$. The stable image therefore has precisely those conjugacy classes as its basis. Comparing dimensions proves

$$
\boxed{\#\{\text{simple }kG\text{-modules}\}
=\#\{\text{p-regular conjugacy classes of }G\}.}
$$

This argument uses dimensions of semilinear images: a bijective scalar Frobenius map preserves dimension, so the usual rank count applies.

In characteristic zero every group element is relevant. Averaging a linear projection onto a [submodule](../../../../../submodule.md) over $G$ makes that projection $G$-equivariant, proving [Maschke's theorem](../../../../../maschke-s-theorem.md) and semisimplicity of $kG$. The same matrix-algebra cocenter calculation now gives $s=\dim C(kG)$, the total number of conjugacy classes.

For the second request, $M$ is a [relative projective module](../../../../../relative-projective-module.md) for $H$ when every $G$-equivariant epimorphism onto $M$ which splits after restriction to $H$ already splits over $G$. Equivalently $M$ is a [direct summand](../../../../../direct-summand.md) of $kG\otimes_{kH}M$, the [induced representation](../../../../../induced-representation.md) of the [restriction of a representation](../../../../../restriction-of-a-representation.md) to $H$. We can verify the defining splitting property directly: if $q:N\twoheadrightarrow M$ has an $H$-linear section $u$, choose representatives $T$ of the left [cosets](../../../../../coset.md) $G/H$ and set

$$
v(m)=\frac1{[G:H]}\sum_{t\in T}t\,u(t^{-1}m).
$$

The sum is independent of representatives by $H$-linearity. Reindexing $gt=t'h$ proves $G$-linearity, while $qv(m)=[G:H]^{-1}\sum_tm=m$. Hence **every $M$ is relatively $H$-projective when the index is invertible in $k$**.

For completeness the canonical induced-module epimorphism $\varepsilon(g\otimes m)=gm$ has the explicit $G$-linear section

$$
\boxed{\sigma(m)=\frac1{[G:H]}\sum_{t\in T}t\otimes t^{-1}m,\qquad \varepsilon\sigma=\operatorname{id}_M.}
$$

It exhibits the promised [direct summand](../../../../../direct-summand.md) and is the [projectivity detected on a subgroup of invertible index](../../../../../projectivity-detected-on-a-subgroup-of-invertible-index.md) construction.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 2](../../paper-2-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

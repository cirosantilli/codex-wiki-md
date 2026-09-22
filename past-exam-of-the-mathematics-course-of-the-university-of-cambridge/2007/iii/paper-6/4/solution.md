<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The ring form of the [Artin–Wedderburn theorem](../../../../../artin-wedderburn-theorem.md) states that the following conditions on a unital [ring](../../../../../ring.md) $R$ are equivalent: $R$ is a [semisimple ring](../../../../../semisimple-ring.md); $R$ satisfies the descending chain condition on [left ideals](../../../../../left-ideal.md) and $J(R)=0$; and

$$
\boxed{R\cong\prod_{i=1}^s M_{n_i}(D_i),}
$$

where $s$ is finite, each $n_i\geq1$, and each $D_i$ is a [division ring](../../../../../division-ring.md). The factors are unique up to permutation and isomorphism. The zero [ring](../../../../../ring.md) may be included as the empty product. This theorem also implies the corresponding right-handed statements.

First prove the implication from the chain condition and zero [Jacobson radical](../../../../../jacobson-radical.md). Among finite intersections of maximal [left ideals](../../../../../left-ideal.md), choose a minimal one, say $L=L_1\cap\cdots\cap L_t$. Such a minimal intersection exists by the descending chain condition. Intersecting with any other maximal [left ideal](../../../../../left-ideal.md) cannot make $L$ smaller, so $L$ is contained in every maximal [left ideal](../../../../../left-ideal.md). Thus $L\subseteq J(R)=0$. It follows that the map of left [modules](../../../../../module-mathematics.md)

$$
R\longrightarrow\bigoplus_{j=1}^t R/L_j
$$

is injective. Each quotient is a [simple module](../../../../../irreducible-module.md).

For completeness, a [submodule](../../../../../submodule.md) $N$ of a finite [direct sum](../../../../../direct-sum.md) $V=\bigoplus_j T_j$ of [simple modules](../../../../../irreducible-module.md) is itself a finite [direct sum](../../../../../direct-sum.md) of [simple modules](../../../../../irreducible-module.md) and is a [direct summand](../../../../../direct-summand.md) of $V$. Choose a sum $W$ of coordinate summands, maximal among those with $N\cap W=0$. For any omitted coordinate summand $T_j$, simplicity gives $T_j\cap(N+W)=0$ or $T_j\subseteq N+W$. In the first case $N\cap(W\oplus T_j)=0$, contradicting maximality; hence every coordinate summand lies in $N+W$. Therefore $V=N\oplus W$. Projection onto $N$ shows $N$ is a finite sum of images of the $T_j$, each image zero or simple. Add these images successively, discarding any image already in the sum: simplicity makes each new intersection zero. This yields a direct-sum decomposition. Applying this argument to the displayed injection proves that the left regular [module](../../../../../module-mathematics.md) is a finite sum of [simple modules](../../../../../irreducible-module.md).

Conversely, if the regular [module](../../../../../module-mathematics.md) is a [direct sum](../../../../../direct-sum.md) of [simple modules](../../../../../irreducible-module.md), that sum is finite because $1$ lies in a finite subsum and generates the whole regular [module](../../../../../module-mathematics.md). Every [left ideal](../../../../../left-ideal.md), being a [submodule](../../../../../submodule.md), has the preceding decomposition and splitting property. Its chain lengths are bounded by the number of simple summands, so the descending chain condition holds. The [Jacobson radical](../../../../../jacobson-radical.md) annihilates every simple summand of the regular [module](../../../../../module-mathematics.md), hence annihilates $1$ and is zero. This identifies the first two conditions.

Write the finite decomposition using pairwise nonisomorphic simple left [modules](../../../../../module-mathematics.md):

$$
{}_RR\cong\bigoplus_{i=1}^s S_i^{n_i}.
$$

Every [simple module](../../../../../irreducible-module.md) is a quotient of $R$, by sending $1$ to any nonzero vector, so this list includes every simple isomorphism class. The [Schur lemma](../../../../../schur-s-lemma.md) gives $\operatorname{Hom}_R(S_i,S_j)=0$ for $i\ne j$, and $E_i=\operatorname{End}_R(S_i)$ is a [division ring](../../../../../division-ring.md): any nonzero endomorphism has zero kernel and full image by simplicity. Consequently

$$
\operatorname{End}_R({}_RR)\cong\prod_{i=1}^sM_{n_i}(E_i).
$$

Every endomorphism of the left regular [module](../../../../../module-mathematics.md) is right multiplication by its value on $1$. Composition reverses multiplication of those values, so the left side is $R^{\mathrm{op}}$. Taking the [opposite ring](../../../../../opposite-ring.md), and using transpose to identify $M_n(E)^{\mathrm{op}}$ with $M_n(E^{\mathrm{op}})$, gives the theorem's decomposition with $D_i=E_i^{\mathrm{op}}$. This keeps the left/right conventions explicit.

Conversely, the standard column [module](../../../../../module-mathematics.md) $D^n$ over $M_n(D)$ is simple: a nonzero coordinate of a vector can be inverted to construct a [matrix](../../../../../matrix.md) sending it to any prescribed vector. The left regular [module](../../../../../module-mathematics.md) decomposes as the sum of its $n$ column ideals, each isomorphic to $D^n$. A finite product of these matrix [rings](../../../../../ring.md) is therefore a [semisimple ring](../../../../../semisimple-ring.md). This proves all implications. For uniqueness, the isomorphism classes of simple [modules](../../../../../module-mathematics.md) and their multiplicities in the regular [module](../../../../../module-mathematics.md) determine the numbers $n_i$ and the division [rings](../../../../../ring.md) $E_i^{\mathrm{op}}$. The multiplicity can also be recovered as the [dimension](../../../../../dimension-vector-space.md) of $\operatorname{Hom}_R(S_i,R)$ as a right $E_i$-[module](../../../../../module-mathematics.md), so it does not depend on the chosen decomposition.

Now let $A=\mathbb C[G]$ for the finite [group](../../../../../group-split.md) $G$. It has [dimension](../../../../../dimension-vector-space.md) $|G|$, with the elements of $G$ as a [basis](../../../../../basis.md), so its [left ideals](../../../../../left-ideal.md) satisfy the descending chain condition by their dimensions. The permitted assumption $J(A)=0$ makes the [Artin–Wedderburn theorem](../../../../../artin-wedderburn-theorem.md) applicable. Its decomposition is a complex-algebra decomposition

$$
A\cong\prod_iM_{n_i}(D_i),
$$

with each $D_i$ finite-dimensional over the central copy of $\mathbb C$. Each such [division algebra](../../../../../division-algebra.md) is just $\mathbb C$. Indeed, for $d\in D_i$, finite dimensionality gives a nonzero polynomial relation $p(d)=0$ with complex coefficients. Factor $p$ into linear factors over $\mathbb C$. Their product at $d$ is zero, so the absence of [zero divisors](../../../../../zero-divisor.md) forces $d-\lambda=0$ for some scalar root $\lambda$. Thus every element is scalar.

The pairwise nonisomorphic simple [modules](../../../../../module-mathematics.md) of $\prod_iM_{n_i}(\mathbb C)$ are the column [modules](../../../../../module-mathematics.md) $\mathbb C^{n_i}$, with all other factors acting as zero. Hence $\dim_{\mathbb C}S_i=n_i$. Taking complex [dimensions](../../../../../dimension-vector-space.md) gives

$$
\boxed{\sum_{i=1}^k(\dim_{\mathbb C}S_i)^2=\sum_{i=1}^kn_i^2=\dim_{\mathbb C}\mathbb C[G]=|G|.}
$$

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 6](../../paper-6-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A [composition series](../../../../../composition-series.md) is a subnormal chain whose nontrivial successive quotients are simple. The [Jordan–Hölder theorem](../../../../../jordan-holder-theorem.md) asserts that any two [composition series](../../../../../composition-series.md) of a [finite group](../../../../../finite-group.md) have the same length and the same multiset of simple factors, up to [isomorphism](../../../../../isomorphism.md). Existence follows by successively choosing maximal proper [normal subgroups](../../../../../normal-subgroup.md) until the identity is reached.

For uniqueness, induct on the [group](../../../../../group-split.md) order. Let $A,B$ be the penultimate terms of two series. If $A=B$, apply induction to that [subgroup](../../../../../subgroup.md) and add the common top factor. If $A\ne B$, their normality and maximality give $AB=G$. Put $C=A\cap B$. The [isomorphism](../../../../../isomorphism.md) theorems give

$$
A/C\cong G/B,\qquad B/C\cong G/A.
$$

Both are simple. Take any [composition series](../../../../../composition-series.md) of $C$. Appending $A$ to it gives a series for $A$, so induction identifies the factors of the original series inside $A$ with the factors of $C$ together with $G/B$. Similarly the factors inside $B$ are those of $C$ together with $G/A$. Adding the respective top factors produces the same multiset in both cases. This proves uniqueness, including multiplicities and length.

A [normal subgroup](../../../../../normal-subgroup.md) $K$ of order two is central because its [automorphism group](../../../../../automorphism-group.md) is trivial. By Jordan–Hölder, a [composition series](../../../../../composition-series.md) through $K$ leaves the simple quotient $G/K\cong A_5$. The image of $Z(G)$ in this quotient is central and hence trivial, since $A_5$ is nonabelian simple. Thus

$$
\boxed{Z(G)=K.}
$$

The [symmetric group](../../../../../symmetric-group.md) $S_5$ has trivial [group center](../../../../../center-of-a-group.md): [conjugation](../../../../../conjugation.md) of each [transposition](../../../../../transposition-permutation.md) by a central [permutation](../../../../../permutation.md) must preserve its two-element support, forcing the [permutation](../../../../../permutation.md) to fix every point. Since its [Jordan–Hölder factors](../../../../../jordan-holder-factor.md) are $A_5$ and $C_2$, a [normal subgroup](../../../../../normal-subgroup.md) of order two would equal that trivial [group center](../../../../../center-of-a-group.md), a contradiction.

Identify $C_2=\{1,-1\}$ and put $D=1\times A_5$ in $C_2\times S_5$. Its three maximal [normal subgroups](../../../../../normal-subgroup.md) are

$$
M_1=C_2\times A_5,\quad M_2=1\times S_5,\quad
M_3=\{(\operatorname{sgn}\sigma,\sigma):\sigma\in S_5\}.
$$

They are the three [kernels](../../../../../kernel-of-a-linear-map.md) of nonzero maps from the [abelianization](../../../../../abelianization.md) $C_2^2$ to $C_2$. There is no quotient $A_5$: a central $C_2$ must map trivially, while $S_5$ has no quotient $A_5$. The latter follows from its [normal subgroups](../../../../../normal-subgroup.md) $1,A_5,S_5$, which can themselves be obtained by intersecting with the simple [subgroup](../../../../../subgroup.md) $A_5$ and using its trivial [centralizer](../../../../../centralizer.md). The complete list of [composition series](../../../../../composition-series.md) is

$$
\boxed{\begin{aligned}
1&<C_2\times1<M_1<C_2\times S_5,\\
1&<D<M_1<C_2\times S_5,\\
1&<D<M_2<C_2\times S_5,\\
1&<D<M_3<C_2\times S_5.
\end{aligned}}
$$

Within $M_1$ the two direct factors are the only maximal [normal subgroups](../../../../../normal-subgroup.md); within each of $M_2,M_3\cong S_5$ the only such [subgroup](../../../../../subgroup.md) is its copy of $A_5$. Hence **there are exactly four series**.

For $S_5\times S_5$, put $D=A_5\times A_5$, $X=A_5\times1$, $Y=1\times A_5$ and

$$
M_L=A_5\times S_5,\quad M_R=S_5\times A_5,\quad
M_D=\{(\sigma,\rho):\operatorname{sgn}\sigma=\operatorname{sgn}\rho\}.
$$

Again these are exactly the maximal [normal subgroups](../../../../../normal-subgroup.md): they are the three cyclic quotient [kernels](../../../../../kernel-of-a-linear-map.md), and there is no simple quotient $A_5$ of the whole product. All series are

$$
\boxed{1<T<D<M<S_5\times S_5\quad(T=X\text{ or }Y,\ M=M_L,M_R,M_D),}
$$

together with

$$
\boxed{1<Y<1\times S_5<M_L<S_5\times S_5,\qquad
1<X<S_5\times1<M_R<S_5\times S_5.}
$$

To verify exhaustiveness, $M_L$ has maximal [normal subgroups](../../../../../normal-subgroup.md) $D$ and $1\times S_5$, and $M_R$ has $D$ and $S_5\times1$. A quotient $A_5$ of a direct product can receive a nontrivial image from only one simple factor, since the images commute and $A_5$ has trivial [group center](../../../../../center-of-a-group.md). The remaining maximal-normal possibility is $M_D$. Its derived [subgroup](../../../../../subgroup.md) is $D$, because both alternating factors are perfect. A hypothetical quotient $A_5$ would project one alternating factor isomorphically and kill the other, but [conjugation](../../../../../conjugation.md) by an odd diagonal element induces an [outer automorphism](../../../../../outer-automorphism-of-a-group.md) on that surviving factor, impossible inside $A_5$. Odd [conjugation](../../../../../conjugation.md) is outer because otherwise an odd [permutation](../../../../../permutation.md) times an even one would centralize $A_5$; a [permutation](../../../../../permutation.md) commuting with every [three-cycle](../../../../../three-cycle.md) fixes every three-element support and is the identity. Thus $D$ is the only maximal [normal subgroup](../../../../../normal-subgroup.md) of $M_D$. Finally the only maximal [normal subgroups](../../../../../normal-subgroup.md) of $D$ are $X,Y$: [normal subgroups](../../../../../normal-subgroup.md) of a product of two centerless [simple groups](../../../../../simple-group.md) are products of the factors, as follows by commutating with each factor. This proves **exactly eight series** and the classification of [composition chains in products with S5](../../../../../composition-chains-in-products-with-s5.md).

For $SL_2(5)$, commuting with both elementary upper and lower [transvections](../../../../../transvection.md) forces a central [matrix](../../../../../matrix.md) to be scalar. A scalar $\lambda I$ has [determinant](../../../../../determinant.md) $\lambda^2$, so

$$
\boxed{Z(SL_2(5))=\{I,-I\}.}
$$

If $g^2=I$, characteristic five makes $g$ diagonalizable with eigenvalues in $\{1,-1\}$. [Determinant](../../../../../determinant.md) one rules out one of each, so the unique nonidentity [involution](../../../../../involution.md) is $-I$. An index-two [subgroup](../../../../../subgroup.md) would have order $60$ and, by the [Cauchy theorem for groups](../../../../../cauchy-theorem-for-groups.md), contain that [involution](../../../../../involution.md) and hence the [group center](../../../../../center-of-a-group.md). Its image in $PSL_2(5)$ would have index two. The simplicity and identification $PSL_2(5)\cong A_5$ are established by the independent [matrix](../../../../../matrix.md) argument in Solution 4; a [simple group](../../../../../simple-group.md) has no proper index-two [subgroup](../../../../../subgroup.md). Therefore **$SL_2(5)$ has no [subgroup](../../../../../subgroup.md) of index two**.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 2](../../paper-2-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

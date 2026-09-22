<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For $n\ge2$, a [cycle type](../../../../../cycle-type.md) $\alpha\vdash n$ lies in $A_n$ exactly when $n-\ell(\alpha)$ is even. Its $S_n$ [conjugacy class](../../../../../conjugacy-class.md) is either one $A_n$ class or two equal-sized classes. Splitting occurs exactly when its [centralizer](../../../../../centralizer.md) in $S_n$ contains no odd [permutation](../../../../../permutation.md). An even-length cycle is itself odd; two equal odd-length cycles can be interchanged by an odd [permutation](../../../../../permutation.md). Conversely, for distinct odd cycle lengths the [centralizer](../../../../../centralizer.md) is a product of cyclic groups of odd order, all contained in $A_n$. Thus **the classes that split are exactly the [partitions of an integer](../../../../../partition-of-an-integer.md) into distinct odd parts**. Repeated fixed points count as repeated parts of length one.

For $n=1$ the group is trivial, with its single [trivial representation](../../../../../trivial-representation.md). Assume $n\ge2$ for the index-two argument that follows. For ordinary [representations](../../../../../group-representation.md) work over $\mathbb C$. Tensoring $S^\lambda$ by the [sign representation](../../../../../sign-representation.md) gives $S^{\lambda'}$. The index-two restriction identity, obtained by [Frobenius reciprocity](../../../../../frobenius-reciprocity.md), is

$$
\left\langle\operatorname{Res}_{A_n}\chi^\lambda,\operatorname{Res}_{A_n}\chi^\mu\right\rangle
=\delta_{\lambda\mu}+\delta_{\lambda'\mu}.
$$

If $\lambda\ne\lambda'$, restriction is [irreducible](../../../../../irreducible-representation.md), and the conjugate pair gives the same [irreducible](../../../../../irreducible-representation.md). If $\lambda=\lambda'$, the norm is two, so restriction is the sum of two distinct [irreducibles](../../../../../irreducible-representation.md). An odd [permutation](../../../../../permutation.md) interchanges them, so both have degree $f^\lambda/2$. Every [irreducible](../../../../../irreducible-representation.md) of $A_n$ occurs in some such restriction: induce it to $S_n$ and choose an [irreducible](../../../../../irreducible-representation.md) constituent, then apply reciprocity. The displayed [inner product](../../../../../inner-product.md) distinguishes all the listed constituents. Hence

$$
\boxed{\operatorname{Irr}(A_n)=\{V^{\{\lambda,\lambda'\}}:\lambda\ne\lambda'\}\ \cup\ \{V^{\lambda,+},V^{\lambda,-}:\lambda=\lambda'\}.}
$$

The first family has degree $f^\lambda$, the second degree $f^\lambda/2$. A choice of labels for the two split classes and constituents fixes the otherwise interchangeable signs.

The one-dimensional [representations](../../../../../group-representation.md) are [characters](../../../../../character-of-a-representation.md) of the [abelianization](../../../../../abelianization.md). For $n\ge5$, simplicity and noncommutativity of $A_n$ make its [abelianization](../../../../../abelianization.md) trivial. For $n=4$, its [commutator subgroup](../../../../../commutator-subgroup.md) is the [Klein four-group](../../../../../klein-four-group.md) and its [abelianization](../../../../../abelianization.md) is $C_3$, giving the three [characters](../../../../../character-of-a-representation.md) obtained by sending a quotient generator to $1,\omega,\omega^2$. For $n=3$, $A_3=C_3$ has the same three [characters](../../../../../character-of-a-representation.md); for $n=1,2$ the group is trivial and has just one. The two additional [linear characters](../../../../../linear-character.md) at $n=4$ are the split constituents of shape $(2,2)$; at $n=3$ they come from $(2,1)$.

Here is a [dimension](../../../../../dimension-vector-space.md) argument that also proves the asserted uniqueness without assuming a classification of small [character](../../../../../character-of-a-representation.md) degrees. Write $f^\lambda$ for the number of [standard tableaux](../../../../../standard-young-tableau.md). Removing the cell containing the largest label gives

$$
f^\lambda=\sum_{\mu\in\lambda^-}f^\mu.
$$

[Hook lengths](../../../../../hook-length.md), or direct [Young tableau](../../../../../young-tableau.md) counting, give the following small cases: for $S_5,S_6$ every non-linear degree is at least $4,5$, respectively. Among non-self-conjugate shapes excluding the row, column and standard pair, the minimum degree at $n=5,6,7$ is respectively $5,5,14$. The self-conjugate shapes at these sizes have half-degrees $3,8,10$, respectively, from $(3,1^2),(3,2,1),(4,1^3)$.

Inductively, for every $n\ge7$, a shape other than the row, column or standard pair has all its one-cell predecessors non-linear. If it has at least two removable corners, each predecessor has degree at least $n-2$, so its degree is at least $2(n-2)$. If it has only one corner, it is a nontrivial rectangle $(a^b)$. Remove that corner and then either of the two corners of $(a^{b-1},a-1)$. For $n\ge8$ these two size-$n-2$ shapes are non-linear, so its degree is at least $2(n-3)$. At $n=7$ there is no nontrivial rectangle. Together with the size-5 and size-6 checks this proves by induction that the standard pair is the only pair of shapes of degree $n-1$ for $n\ge7$, and that every other non-linear degree is larger.

We must additionally exclude a self-conjugate shape of degree $2(n-1)$, since its restriction splits. For $n\ge8$, if such a shape has at least three corners, the preceding lower bound gives $f^\lambda\ge3(n-2)>2(n-1)$. With two corners, its predecessors are a conjugate pair and are not standard shapes; the bounds just proved give $f^\lambda\ge4(n-4)>2(n-1)$. With one corner it is a square $(a^a)$. For $a\ge4$, the two size-$n-2$ predecessors obtained after two removals are nonstandard, giving $f^\lambda\ge4(n-5)>2(n-1)$. The remaining square $(3^3)$ has degree $42>16$ by the [hook-length formula](../../../../../hook-length-formula.md). The size-7 self-conjugate case has degree $20>12$. This excludes both smaller split degrees and equality with the standard degree.

It follows that the lowest non-linear ordinary degree is **$3$ for $A_4$ and $n-1$ for every $n\ge6$**. For $A_1,A_2,A_3$ no non-linear [irreducible](../../../../../irreducible-representation.md) exists. The excluded case $A_5$ has lowest degree $3$, although its standard degree-$4$ [representation](../../../../../group-representation.md) is unique. At $A_6$ there are two degree-$5$ [irreducibles](../../../../../irreducible-representation.md), from the standard conjugate pair and the pair $(3,3),(2,2,2)$.

Finally, for every $n\ge7$ the preceding proof gives a unique degree-$n-1$ [irreducible](../../../../../irreducible-representation.md), namely the restriction of $S^{(n-1,1)}$. The small cases $n=4,5$ have unique degree $3,4$, respectively, and $A_2$ has its unique trivial degree-$1$ [representation](../../../../../group-representation.md). These prove exactly the requested uniqueness range; the omitted cases $n=3,6$ genuinely fail.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 4](../../paper-4-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

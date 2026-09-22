<h1 id="2d/solution">Solution</h1>

↑ **Parent:** [2D](../2d.md)

A [cyclic group](../../../../../cyclic-group.md) has one [generator of a group](../../../../../generator-of-a-group.md): $G=\langle a\rangle=\{a^j:j\in\mathbb Z\}$. An [abelian group](../../../../../abelian-group.md) has $xy=yx$ for every pair of elements. Powers of one element commute because $a^ra^s=a^{r+s}=a^{s+r}=a^sa^r$, so **every [cyclic group](../../../../../cyclic-group.md) is [Abelian](../../../../../abelian-group.md)**. The [Klein four-group](../../../../../klein-four-group.md) $C_2\times C_2$ is [Abelian](../../../../../abelian-group.md) but is not a [cyclic group](../../../../../cyclic-group.md): every nonidentity element has order two, whereas a [generator of a group](../../../../../generator-of-a-group.md) for a four-element [cyclic group](../../../../../cyclic-group.md) would have order four.

Fix a [generator of a group](../../../../../generator-of-a-group.md) $x$ of $C_n$. A [group homomorphism](../../../../../group-homomorphism.md) is determined by $g=\phi(x)$ because $\phi(x^j)=g^j$, and the relation $x^n=1$ forces $g^n=1$. Conversely, such a $g$ defines $\phi(x^j)=g^j$: exponents differing by a multiple of $n$ give the same value, and addition of exponents verifies the [group homomorphism](../../../../../group-homomorphism.md) law. Thus the [homomorphism from a finite cyclic group](../../../../../homomorphism-from-a-finite-cyclic-group.md) correspondence is

$$
\boxed{\operatorname{Hom}(C_n,G)\ \longleftrightarrow\ \{g\in G:g^n=1\}.}
$$

For $S_4$, the order of a [permutation](../../../../../permutation.md) is the [least common multiple](../../../../../least-common-multiple.md) of its disjoint cycle lengths. The condition $\sigma^4=1$ allows identity, [transpositions](../../../../../transposition-permutation.md), two disjoint [transpositions](../../../../../transposition-permutation.md), and four-cycles. The **sixteen homomorphisms** are $\phi_\sigma(x^j)=\sigma^j$, with the full list of possible generator images

$$
\boxed{\begin{gathered}
1;\\
(12),(13),(14),(23),(24),(34);\\
(12)(34),(13)(24),(14)(23);\\
(1234),(1243),(1324),(1342),(1423),(1432).
\end{gathered}}
$$

The remaining eight elements of the [symmetric group](../../../../../symmetric-group.md) are [three-cycles](../../../../../three-cycle.md) and do not qualify.

## ↑ Ancestors (10)

1. [2D](../2d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

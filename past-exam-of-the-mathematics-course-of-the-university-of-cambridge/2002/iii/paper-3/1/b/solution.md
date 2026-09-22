<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Modulo two the [polynomial](../../../../../../polynomial-split.md) becomes $h=X^5+X^2+1$. It has neither zero nor one as a root. The only irreducible quadratic over $\mathbb F_2$ is $X^2+X+1$; modulo it, $X^3=1$ and $h\equiv1$. A reducible quintic has a factor of degree at most two, so $h$ is irreducible. It is also separable: $h'=X^4$, which is coprime to $h$. Thus the rational [polynomial](../../../../../../polynomial-split.md) is irreducible, and its group $G\leq S_5$ is transitive.

Modulo three there is the exact factorization

$$
f=(X^2+1)(X^3+2X+1).
$$

The quadratic has no root. The cubic takes value one at each of $0,1,2$, so it too has no root and is irreducible. The two factors are distinct and coprime. The [Frobenius cycle type](../../../../../../frobenius-cycle-type.md) therefore supplies an element with disjoint cycles of lengths two and three. Its cube is a single [transposition](../../../../../../transposition-permutation.md).

A transitive action of prime degree is primitive: a block size divides five, so the only sizes are one and five. To finish without classifying all degree-five groups, apply the [primitive group with a transposition](../../../../../../primitive-group-with-a-transposition.md) argument. Form the graph of all conjugate [transpositions](../../../../../../transposition-permutation.md) in $G$. Its connected components are blocks, so it is connected. [Transpositions](../../../../../../transposition-permutation.md) along the edges of a connected graph generate every [transposition](../../../../../../transposition-permutation.md): along a path, conjugating adjacent swaps yields the swap of its endpoints. Hence they generate $S_5$, and

$$
\boxed{\operatorname{Gal}(f,\mathbb Q)=S_5.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

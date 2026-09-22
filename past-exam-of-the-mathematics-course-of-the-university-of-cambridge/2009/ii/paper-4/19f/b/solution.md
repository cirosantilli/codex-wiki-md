<h1 id="19f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [induced character](../../../../../../induced-character.md) construction extends any [class function](../../../../../../class-function.md) $\psi$ on $H$ by

$$
\operatorname{Ind}_H^G\psi(g)=\frac1{|H|}\sum_{x\in G:\,x^{-1}gx\in H}\psi(x^{-1}gx).
$$

[Frobenius reciprocity](../../../../../../frobenius-reciprocity.md) for class functions is $\langle\operatorname{Ind}_H^G\psi,\chi\rangle_G=\langle\psi,\operatorname{Res}_H^G\chi\rangle_H$. It follows directly by substituting this sum into the left [inner product](../../../../../../inner-product.md), writing $g=xhx^{-1}$, and using the conjugacy invariance of $\chi$. If $\psi$ is a [character](../../../../../../character-of-a-representation.md), its [inner product](../../../../../../inner-product.md) with every restricted [irreducible character](../../../../../../irreducible-character.md) is a nonnegative integer, a multiplicity in its complete reducible decomposition. Expanding in the [orthonormal](../../../../../../orthonormal-set.md) irreducible-character basis therefore makes $\operatorname{Ind}\psi$ a nonnegative integer sum of irreducible characters: **it is a [character](../../../../../../character-of-a-representation.md) of $G$**.

If $U$ affords $\psi$, a concrete [induced representation](../../../../../../induced-representation.md) is $\mathbb C[G]\otimes_{\mathbb C[H]}U$, with $G$ acting by left multiplication on the first factor. Choosing [coset](../../../../../../coset.md) representatives decomposes it into $[G:H]$ copies of $U$. An element $g$ permutes these copies; only fixed [cosets](../../../../../../coset.md) contribute [trace](../../../../../../matrix-trace.md), and the contribution from $xH$ is $\psi(x^{-1}gx)$. Summing fixed [cosets](../../../../../../coset.md) gives exactly the displayed induced [class function](../../../../../../class-function.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [19F](../../19f.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

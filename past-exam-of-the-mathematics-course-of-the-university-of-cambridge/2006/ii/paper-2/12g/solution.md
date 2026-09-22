<h1 id="12g/solution">Solution</h1>

↑ **Parent:** [12G](../12g.md)

A cyclic binary code is a [linear subspace](../../../../../vector-subspace.md) of $\mathbb F_2^n$ invariant under cyclic shifts. Identify a word with its coefficient [polynomial](../../../../../polynomial-split.md) in $\mathbb F_2[X]/(X^n-1)$. Multiplication by $X$ is the shift, so the code is precisely an [ideal](../../../../../ideal.md) of that [quotient ring](../../../../../quotient-ring.md). Its inverse image in the [polynomial ring](../../../../../polynomial-ring.md) is a [principal ideal](../../../../../principal-ideal.md) $(g)$ containing $(X^n-1)$; its unique monic generator divides $X^n-1$. Conversely each monic divisor generates such an [ideal](../../../../../ideal.md). Thus the bijection is with **monic divisors**; $g=1$ gives the full code and $g=X^n-1$ the [zero code](../../../../../zero-code.md).

For odd $n$, some $m$ has $n\mid2^m-1$, so the cyclic multiplicative group of $\mathbb F_{2^m}$ contains a primitive $n$th root $\alpha$. If a nonzero word with the specified roots had weight $w<\delta$, write its nonzero positions as $r_1,\ldots,r_w$. The root equations give

$$
\sum_{j=1}^w c_j(\alpha^{r_j})^i=0\quad(1\le i\le w).
$$

Their matrix has [determinant](../../../../../determinant.md) $\prod_j\alpha^{r_j}\prod_{j<l}(\alpha^{r_l}-\alpha^{r_j})\ne0$, by the Vandermonde formula and distinctness of the positions. Thus all coefficients would vanish, a contradiction. Hence **[minimum distance](../../../../../minimum-distance-of-a-code.md) is at least $\delta$**.

For $n=7$, choose $\alpha$ with [minimal polynomial](../../../../../minimal-polynomial.md) $X^3+X+1$. The roots $\alpha,\alpha^2$ force also the conjugate $\alpha^4$, giving this cubic as generator. Its degree gives dimension four and its weight gives distance exactly three. Expressing $c(\alpha)=0$ in a basis of $\mathbb F_8$ gives a [parity-check matrix](../../../../../parity-check-matrix.md) with the seven distinct nonzero vectors of $\mathbb F_2^3$ as columns. This is **the binary $[7,4,3]$ [Hamming code](../../../../../hamming-code.md)**. Its sixteen disjoint radius-one balls have $16(1+7)=128$ words, so one-error correction is perfect. The other primitive cubic produces an equivalent coordinate-permuted code.

## ↑ Ancestors (10)

1. [12G](../12g.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

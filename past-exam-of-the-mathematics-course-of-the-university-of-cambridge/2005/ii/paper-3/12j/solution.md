<h1 id="12j/solution">Solution</h1>

↑ **Parent:** [12J](../12j.md)

A linear length-$n$ [cyclic code](../../../../../cyclic-code.md) is a subspace closed under cyclic coordinate shifts. Identify a word with its [polynomial](../../../../../polynomial-split.md) modulo $X^n-1$; multiplying by $X$ performs the shift. Thus a cyclic code is an [ideal](../../../../../ideal.md) of $\mathbb F_q[X]/(X^n-1)$. Its preimage in the [polynomial](../../../../../polynomial-split.md) ring is an [ideal](../../../../../ideal.md) containing $X^n-1$, so the [Euclidean algorithm](../../../../../euclidean-algorithm.md) gives a unique monic generator $g$ dividing $X^n-1$. The [generator polynomial of a cyclic code](../../../../../generator-polynomial-of-a-cyclic-code.md) is $g$ and the [check polynomial of a cyclic code](../../../../../check-polynomial-of-a-cyclic-code.md) is $h=(X^n-1)/g$; a word lies in the code exactly when $hc\equiv0\pmod{X^n-1}$.

For the binary length-seven code, the given $h$ factors with

$$
\boxed{g(X)=X^3+X+1,\qquad (X^3+X+1)(X^4+X^2+X+1)=X^7+1.}
$$

This cubic has no binary root and is irreducible. Let $\alpha$ be its root in $\mathbb F_8$. Since the nonzero multiplicative group has [prime](../../../../../prime-number.md) order seven and $\alpha\ne1$, its seven powers enumerate all nonzero elements. The condition $c(\alpha)=0$ gives a three-row binary parity-check [matrix](../../../../../matrix.md) whose columns are precisely the seven nonzero vectors of $\mathbb F_2^3$. This is [Hamming's code](../../../../../hamming-code.md) in a cyclic coordinate order. It has dimension four, and minimum distance three: no one or two distinct nonzero columns sum to zero, while $g$ itself has weight three. Its sixteen radius-one balls have total size $16(1+7)=128$, confirming the original perfect Hamming code.

It actually contains its [dual code](../../../../../dual-code.md) in this coordinate order. Each parity-check row has four ones, and any two distinct rows have two simultaneous ones, so $HH^T=0$ over $\mathbb F_2$. The row space $C^\perp$ therefore lies in $\ker H=C$. Equivalently the dual generator is the reciprocal check [polynomial](../../../../../polynomial-split.md)

$$
h^*(X)=X^4+X^3+X^2+1=(X+1)g(X),
$$

which is divisible by $g$. Hence **there is a three-dimensional subcode equal to the dual**, and in any other coordinate order it is equivalent to that dual.

## ↑ Ancestors (10)

1. [12J](../12j.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

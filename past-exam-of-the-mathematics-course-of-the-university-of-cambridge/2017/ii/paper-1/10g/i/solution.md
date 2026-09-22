<h1 id="10g/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [linear code](../../../../../../linear-code.md) of length $n$ and rank $k$ is a $k$-dimensional [linear subspace](../../../../../../vector-subspace.md) of $\mathbb F_2^n$. The [Hamming weight](../../../../../../hamming-weight.md) of a vector counts its nonzero coordinates. Thus the sum of the coefficients of the [weight enumerator](../../../../../../weight-enumerator.md) is the number of codewords:

$$
\boxed{W_C(1,1)=2^k}.
$$

Since the zero vector is the unique word of weight zero, $W_C(0,1)=1$. Symmetry of the enumerator therefore implies $W_C(1,0)=1$. Conversely $W_C(1,0)=1$ means that the all-one vector $\mathbf1$ belongs to $C$. Translation $x\mapsto x+\mathbf1$ is then a bijection of $C$ which replaces weight $j$ by $n-j$, proving the [polynomial](../../../../../../polynomial-split.md) symmetry. For length zero the same conclusion holds with the unique empty vector.

The [dual code](../../../../../../dual-code.md) is $C^\perp=\{y:x\cdot y=0\text{ for every }x\in C\}$, using the standard bilinear form over $\mathbb F_2$. If $y\in C^\perp$, each summand of the character sum equals one. Otherwise choose $x_0\in C$ with $x_0\cdot y=1$; replacing $x$ by $x+x_0$ permutes the summands and reverses their sign. The sum equals its own negative and must be zero. Consequently

$$
\boxed{\sum_{x\in C}(-1)^{x\cdot y}=2^k\mathbf1_{\{y\in C^\perp\}}}.
$$

This is [character orthogonality](../../../../../../character-orthogonality.md) for the additive [group](../../../../../../group-split.md) of the code.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [10G](../../10g.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

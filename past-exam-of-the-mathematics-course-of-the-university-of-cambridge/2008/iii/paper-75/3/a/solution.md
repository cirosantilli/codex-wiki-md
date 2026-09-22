<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A nontrivial example is $f_n=T_{n+1}$, the [Chebyshev polynomial](../../../../../../chebyshev-polynomial.md) characterized by $T_{n+1}(\cos\theta)=\cos((n+1)\theta)$. Its [supremum norm](../../../../../../supremum-norm.md) is one. At the $n+2$ points $\cos(j\pi/(n+1))$, $0\le j\le n+1$, its values alternate between $1$ and $-1$; reversing their order gives increasing nodes with the same alternation.

The zero [polynomial](../../../../../../polynomial-split.md) therefore satisfies the [Chebyshev alternation theorem](../../../../../../equioscillation-theorem.md) for degree at most $n$, so $E_n(f_n)=1$. Since the smaller [polynomial](../../../../../../polynomial-split.md) space is contained in the larger one, $E_{n-1}(f_n)\ge1$; the zero [polynomial](../../../../../../polynomial-split.md) is feasible in the smaller space as well, giving the reverse inequality. Hence

$$
\boxed{f_n=T_{n+1},\qquad E_{n-1}(f_n)=E_n(f_n)=1.}
$$

A constant [function](../../../../../../function-split.md) would also give equality with both errors zero, but this example shows that equality can occur at a positive approximation error.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 75](../../../paper-75-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

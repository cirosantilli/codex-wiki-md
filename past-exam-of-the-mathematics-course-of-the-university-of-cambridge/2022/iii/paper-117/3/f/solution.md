<h1 id="3/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Assume $RT=N$. To beat the trivial bound $\|b\|_2\|c\|_2N^{1/2}$ by $(\log N)^{-A}$, it is enough to make every term in the parentheses of part e smaller than a sufficiently larger negative power of $\log N$, allowing for the prefactor $(\log q)(\log N)^{O(1)}$.

Choose the splitting parameter $X=(\log N)^B$ with $B$ large in terms of $A$. It then suffices, for a still larger constant $C=C(A,B)$, that

$$
T\geq(\log N)^C,qquad
R\geq X(\log N)^C,qquad
q\geq X(\log N)^C,qquad
Xq\leq\frac{N^2}{(\log N)^C}.
$$

Indeed, these four conditions control respectively the last, third, second, and fourth terms, while the choice of $X$ controls the first. Equivalently, away from polylogarithmic neighborhoods of the endpoints, the estimate gives a logarithmic saving whenever

$$
R,T,q,\frac{N^2}{q}
$$

are all sufficiently large powers of $\log N$, with $R$ also larger than the chosen divisor cutoff $X$ by such a power. This is the Type II range used after [Vaughan identity](../../../../../../vaughan-s-identity.md).

## ↑ Ancestors (11)

1. [F](../f.md)
2. [3](../../3.md)
3. [Paper 117](../../../paper-117-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

<h1 id="9f/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

To prove that [trace is the unique normalized cyclic linear functional](../../../../../../trace-is-the-unique-normalized-cyclic-linear-functional.md), let $E_{ij}$ be the [matrix units](../../../../../../matrix-unit.md). For $i\ne j$, $E_{ii}E_{ij}=E_{ij}$ whereas $E_{ij}E_{ii}=0$, so the assumed identity for the [linear functional](../../../../../../linear-functional.md) gives $f(E_{ij})=0$. Also, $E_{ij}E_{ji}=E_{ii}$ and $E_{ji}E_{ij}=E_{jj}$, giving $f(E_{ii})=f(E_{jj})$. Write this common value as $c$. Since the [matrix units](../../../../../../matrix-unit.md) form a [basis](../../../../../../basis.md),

$$
\boxed{f(A)=\sum_{i,j}a_{ij}f(E_{ij})=c\sum_i a_{ii}=c\operatorname{Tr}(A).}
$$

For $n=1$ the same conclusion follows immediately from the one-dimensional [basis](../../../../../../basis.md) $E_{11}$. Finally, $f(I)=nc$; if this equals $n$, then $c=1$ over either specified field. **The normalization makes $f$ exactly the trace.**

## ↑ Ancestors (11)

1. [C](../c.md)
2. [9F](../../9f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

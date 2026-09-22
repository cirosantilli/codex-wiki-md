<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $B=D+K$, where $D$ has $A$ in each diagonal block and zero elsewhere, while $K$ has $I$ immediately above the diagonal and zero elsewhere. These [block matrices](../../../../../block-matrix.md) satisfy $DK=KD$: either product has $A$ immediately above the diagonal. Also, $K^i$ has $I$ on its $i$th superdiagonal and is zero elsewhere.

The [binomial theorem for commuting matrices](../../../../../binomial-theorem-for-commuting-matrices.md) therefore yields

$$
B^j=\sum_{r=0}^j\binom jrD^{j-r}K^r.
$$

Only $r=i$ can contribute to block $(k,k+i)$, provided that block lies in the [matrix](../../../../../matrix.md). Hence

$$
\boxed{(B^j)_{k,k+i}=\begin{cases}
0,&j<i,\\
\binom ji A^{j-i},&j\geq i.
\end{cases}}
$$

Thus $\beta_{i,j}=\binom ji$, interpreted as an element of the [field](../../../../../field.md). The formula remains valid in positive [field characteristic](../../../../../characteristic-of-a-field.md): some of these coefficients can then vanish. This possibility matters in the next part.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the linear algebra course of the University of Oxford](../../../../split.md)
6. [Linear algebra course of the University of Oxford](../../../../../linear-algebra-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

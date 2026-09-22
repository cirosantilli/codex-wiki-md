<h1 id="18i/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $F=L^G$ and $n=|G|$. The [automorphism-count bound for a finite field extension](../../../../../../automorphism-count-bound-for-a-finite-field-extension.md) gives

$$
n\leq[L:F].
$$

For the reverse inequality, let $x_1,\ldots,x_m$ be linearly independent over $F$. We claim that the $n\times m$ matrix

$$
M=(g(x_j))_{g\in G,\,1\leq j\leq m}
$$

has linearly independent columns over $L$. If not, choose a nonzero relation

$$
\sum_jc_jg(x_j)=0\qquad\text{for every }g\in G
$$

with the fewest nonzero coefficients, and normalize one coefficient to $c_1=1$. Applying $h\in G$ and reindexing the rows gives another relation with coefficients $h(c_j)$. Subtracting eliminates the first term, so minimality forces $h(c_j)=c_j$ for every $h$ and $j$. Thus every $c_j\in F$. The row for the identity automorphism then contradicts the $F$-linear independence of the $x_j$.

Therefore $m\leq n$. Taking an $F$-basis of $L$ gives $[L:F]\leq n$, and hence

$$
\boxed{[L:L^G]=|G|.}
$$

This proves the degree assertion in the [Artin fixed-field theorem](../../../../../../artin-fixed-field-theorem.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [18I](../../18i.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

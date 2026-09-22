<h1 id="1e/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $E_{rs}$ be the [matrix unit](../../../../../../matrix-unit.md) with its only nonzero entry in row $r$, column $s$. For

$$
A=\operatorname{diag}(1,2,\ldots,n),
$$

one has

$$
AE_{rs}=rE_{rs},
\qquad
E_{rs}A=sE_{rs}.
$$

Therefore

$$
\boxed{\phi_A(E_{rs})=(r-s)E_{rs}}.
$$

The $n^2$ matrix units form an [eigenbasis](../../../../../../eigenbasis.md), with $E_{rs}$ having eigenvalue $r-s$. The zero eigenspace consists exactly of the diagonal matrices and has dimension $n$. The [rank-nullity theorem](../../../../../../rank-nullity-theorem.md) now gives

$$
\boxed{\operatorname{rank}\phi_A=n^2-n}.
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1E](../../1e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

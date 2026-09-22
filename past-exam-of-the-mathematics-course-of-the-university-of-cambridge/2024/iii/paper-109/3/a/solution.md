<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $D(a)$ denote the stated constant term and suppose every $a_i>0$. The rational identity

$$
\sum_{k=1}^n
\prod_{j\ne k}\left(1-\frac{X_k}{X_j}\right)^{-1}=1
$$

can be verified after clearing denominators, or by [Lagrange interpolation](../../../../../../lagrange-polynomial.md). Multiplying it by the Dyson product and taking constant terms gives the recursion

$$
D(a_1,\ldots,a_n)=
\sum_{k=1}^nD(a_1,\ldots,a_k-1,\ldots,a_n).
$$

The [multinomial coefficient](../../../../../../multinomial-coefficient.md)

$$
M(a)=\frac{(a_1+\cdots+a_n)!}{a_1!\cdots a_n!}
$$

obeys the same recursion by the multinomial form of [Pascal's identity](../../../../../../pascal-s-rule.md).

If $a_k=0$, taking the constant term in $X_k$ forces the zero term from every factor involving $X_k$ and reduces the expression to the $(n-1)$-variable Dyson product with $a_k$ omitted. The same boundary reduction holds for $M(a)$. Finally $D(0,\ldots,0)=M(0,\ldots,0)=1$. Induction on $n$ and on $a_1+\cdots+a_n$ therefore proves the [Dyson constant-term identity](../../../../../../dyson-constant-term-identity.md)

$$
\boxed{D(a)=M(a)}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 109](../../../paper-109-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

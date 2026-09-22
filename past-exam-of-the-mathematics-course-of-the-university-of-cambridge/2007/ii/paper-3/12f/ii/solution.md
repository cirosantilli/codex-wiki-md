<h1 id="12f/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $\xi_{n+1}=a_{n+1}+1/(a_{n+2}+\cdots)$ be the complete quotient. Iterating the fractional-linear formula for a [continued fraction](../../../../../../continued-fraction.md) gives

$$
x=\frac{p_n\xi_{n+1}+p_{n-1}}{q_n\xi_{n+1}+q_{n-1}}.
$$

The supplied [determinant](../../../../../../determinant.md) identity and $\xi_{n+1}>a_{n+1}$ therefore imply

$$
\boxed{\left|x-\frac{p_n}{q_n}\right|
=\frac1{q_n(q_n\xi_{n+1}+q_{n-1})}
<\frac1{q_nq_{n+1}}.}
$$

The positive partial quotients ensure increasing denominators tending to infinity; the same [determinant](../../../../../../determinant.md) identity makes the even and odd convergents nested, giving their common limit $x$. The displayed formula follows by passing to the limit in the finite-tail identity.

An explicit choice is **$a_n=10^{n!}$ for every $n\geq1$**. The recurrence gives $q_n\leq\prod_{j=1}^n(a_j+1)\leq2^n10^{\sum_{j=1}^nj!}$. For $n\geq2$, $\sum_{j=1}^nj!\leq2n!$, so $\log_{10}q_n\leq3n!$. Consequently $a_{n+1}=10^{(n+1)!}\geq q_n^{(n+1)/3}$ and

$$
0<\left|x-\frac{p_n}{q_n}\right|<q_n^{-2-(n+1)/3}.
$$

First $x$ is irrational: if $x=P/Q$, the nonzero difference from a convergent is at least $1/(Qq_n)$, contradicting the error bound once $q_{n+1}>Q$. If $x$ were algebraic of any fixed degree $d$, the last displayed upper bound would eventually be smaller than $c/q_n^d$ for the positive constant in part (i), since $q_n\to\infty$. This contradicts the [Liouville approximation theorem](../../../../../../liouville-approximation-theorem.md). Thus **this explicit [continued fraction](../../../../../../continued-fraction.md) is transcendental**.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [12F](../../12f.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

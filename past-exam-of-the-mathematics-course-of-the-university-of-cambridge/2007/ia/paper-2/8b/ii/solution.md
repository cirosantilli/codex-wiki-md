<h1 id="8b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The homogeneous sequences are again $(-2)^k$ and $(-3)^k$. A particular solution $D2^k$ has left-hand side $10D2^k$, so $D=1/10$. Consequently $y_k=A(-2)^k+B(-3)^k+2^k/10$. The two [initial conditions](../../../../../../initial-condition.md) require $A+B=9/10$ and $-2A-3B=4/5$, giving $A=7/2$ and $B=-13/5$. Thus

$$
\boxed{y_k=\frac{35(-2)^k-26(-3)^k+2^k}{10}.}
$$

The [linear recurrence relation](../../../../../../linear-recurrence-relation.md) can be rearranged as $y_{k+1}=2^k-5y_k-6y_{k-1}$. Starting with the two integer values, [mathematical induction](../../../../../../mathematical-induction.md) proves that every $y_k$ for $k\geq0$ is an integer. For $n\geq1$, the closed form gives

$$
2^n-26(-3)^n=10y_n-35(-2)^n.
$$

The first term on the right is divisible by ten; the second is too, because $(-2)^n$ supplies a factor two and $35$ supplies a factor five. Therefore **$10$ divides $2^n-26(-3)^n$ for every positive integer $n$**. The positivity condition matters: at $n=0$ the expression is $-25$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [8B](../../8b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

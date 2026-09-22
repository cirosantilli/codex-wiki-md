<h1 id="6d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The special [binomial theorem](../../../../../../binomial-theorem.md)

$$
(1+t)^n=\sum_{k=0}^n\binom nk t^k
$$

follows by [mathematical induction](../../../../../../mathematical-induction.md). Multiplication of the formula for $n$ by $1+t$ and collection of the coefficient of $t^k$ uses Pascal's identity from part (a).

Termwise integration from $0$ to $1$ gives

$$
\boxed{
\sum_{k=0}^n\frac1{k+1}\binom nk
=\int_0^1(1+t)^n\,dt
=\frac{2^{n+1}-1}{n+1}}.
$$

Replacing $t$ by $-t$ gives

$$
\boxed{
\sum_{k=0}^n\frac{(-1)^k}{k+1}\binom nk
=\int_0^1(1-t)^n\,dt
=\frac1{n+1}}.
$$

Finally,

$$
\sum_{k=1}^n\frac{(-1)^{k+1}}k\binom nk
=\int_0^1\frac{1-(1-x)^n}{x}\,dx.
$$

Writing $y=1-x$ and using the finite [geometric series](../../../../../../geometric-series.md),

$$
\frac{1-y^n}{1-y}=1+y+\cdots+y^{n-1},
$$

turns this into

$$
\boxed{\sum_{j=0}^{n-1}\int_0^1y^j\,dy
=1+\frac12+\cdots+\frac1n}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6D](../../6d.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

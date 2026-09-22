<h1 id="2e/solution">Solution</h1>

↑ **Parent:** [2E](../2e.md)

For the odd-square sum, the initial case $n=1$ gives $1=(4-1)/3$. Assume the formula at $n$. Adding the next square gives

$$
\sum_{j=1}^{n+1}(2j-1)^2
=\frac{4n^3-n}{3}+(2n+1)^2
=\frac{4n^3+12n^2+11n+3}{3}
=\frac{4(n+1)^3-(n+1)}3.
$$

The initial case and this [induction](../../../../../mathematical-induction.md) step prove $\boxed{\sum_{j=1}^n(2j-1)^2=(4n^3-n)/3}$ for every positive [integer](../../../../../integer.md) $n$.

For the [divisibility](../../../../../divisibility.md) assertion, $1^3+5\cdot1=6$. The change when $n$ is replaced by $n+1$ is

$$
(n+1)^3+5(n+1)-(n^3+5n)=3n(n+1)+6.
$$

One of the consecutive [integers](../../../../../integer.md) $n,n+1$ is even, so the displayed change is divisible by $6$. If $n^3+5n$ is divisible by $6$, its successor is too. Thus [induction](../../../../../mathematical-induction.md) proves $\boxed{6\mid n^3+5n}$ for every $n\geq1$.

## ↑ Ancestors (10)

1. [2E](../2e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

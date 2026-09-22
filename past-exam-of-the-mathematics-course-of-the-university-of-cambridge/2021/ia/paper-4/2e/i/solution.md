<h1 id="2e/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [Fibonacci recurrence](../../../../../../fibonacci-number.md) gives

$$
a_{n+1}=\frac{F_{n+2}}{F_{n+1}}
=1+\frac{F_n}{F_{n+1}}=1+\frac1{a_n}.
$$

The map $x\mapsto1+1/x$ is strictly decreasing for $x>0$. Since $a_3=2\geq a_1=1$, applying this decreasing map reverses each inequality and proves by [mathematical induction](../../../../../../mathematical-induction.md) that

$$
(-1)^na_{n+2}\leq(-1)^na_n.
$$

Taking even $n$ shows $a_{2n+2}\leq a_{2n}$, so $(a_{2n})$ is a [decreasing sequence](../../../../../../monotone-sequence.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2E](../../2e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

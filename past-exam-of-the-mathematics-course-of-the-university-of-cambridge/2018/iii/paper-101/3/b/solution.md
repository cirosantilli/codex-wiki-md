<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

**False.** In the [polynomial ring](../../../../../../polynomial-ring.md) $R=k[x,y]$ over a [field](../../../../../../field.md), take

$$
P=(x,y),\qquad I=(x,y^2).
$$

The [ideal](../../../../../../ideal.md) $P$ is a [maximal ideal](../../../../../../maximal-ideal.md), with [quotient ring](../../../../../../quotient-ring.md) $R/P\cong k$. Also

$$
R/I\cong k[y]/(y^2).
$$

In this last [ring](../../../../../../ring.md), an element with nonzero constant term is a [unit](../../../../../../unit-in-a-ring.md), and an element with zero constant term is a multiple of $y$ and has square zero. Thus every [zero divisor](../../../../../../zero-divisor.md) is a [nilpotent element](../../../../../../nilpotent.md). This is equivalent to $I$ being a [primary ideal](../../../../../../primary-ideal.md): a zero product in the [quotient ring](../../../../../../quotient-ring.md) with one nonzero factor forces the other factor to be nilpotent. Its [radical of an ideal](../../../../../../radical-of-an-ideal.md) is $P$, so $I$ is $P$-primary.

However, $y\notin I$, so $I\ne P$. Moreover $x\in I$ while $x\notin P^2$, since every polynomial in $P^2$ has no term of total degree one. For every $n\geq2$, $P^n\subseteq P^2$, so $I\ne P^n$. Hence

$$
\boxed{(x,y^2)\text{ is }(x,y)\text{-primary but is not a power of }(x,y).}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 101](../../../paper-101-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

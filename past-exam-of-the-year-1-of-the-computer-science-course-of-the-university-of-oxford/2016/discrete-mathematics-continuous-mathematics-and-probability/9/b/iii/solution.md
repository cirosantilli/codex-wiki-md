<h1 id="9/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Write $F_X(x)=\mathbb P(X\leq x)$ and $F_Y(x)=\mathbb P(Y\leq x)$. For $0\leq x\leq\mu$, the factor $t/\mu$ is at most one throughout $0\leq t\leq x$, so

$$
F_Y(x)=\int_0^x\frac t\mu f(t)\,dt\leq\int_0^x f(t)\,dt=F_X(x).
$$

For $x>\mu$, compare the tails instead: $t/\mu\geq1$ throughout $t\geq x$, giving

$$
1-F_Y(x)=\int_x^\infty\frac t\mu f(t)\,dt\geq\int_x^\infty f(t)\,dt=1-F_X(x).
$$

Rearranging proves

$$
\boxed{\mathbb P(Y\leq x)\leq\mathbb P(X\leq x)\quad(x\geq0).}
$$

This is [stochastic domination](../../../../../../stochastic-domination-of-probability-measures.md) of $X$ by its [size-biased distribution](../../../../../../size-biased-distribution.md). The proof needs only the finite positive [mean](../../../../../../expected-value-split.md), not the finite [variance](../../../../../../variance-split.md) assumed in (ii).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [9](../../../9.md)
4. [Discrete mathematics, continuous mathematics and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2016](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)

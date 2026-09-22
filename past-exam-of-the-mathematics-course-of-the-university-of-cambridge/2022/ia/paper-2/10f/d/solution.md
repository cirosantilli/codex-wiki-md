<h1 id="10f/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

When $r$ red marbles remain, the next draw reduces their number with probability $r/n$. The waiting time $W_r$ for that reduction has a [geometric distribution](../../../../../../geometric-distribution.md) on $\{1,2,\ldots\}$ and therefore

$$
G_{W_r}(s)
=\frac{(r/n)s}{1-(1-r/n)s}
=\frac{rs}{n-(n-r)s}.
$$

The successive waiting times are independent, and

$$
T=W_n+W_{n-1}+\cdots+W_1.
$$

Using the product rule for probability-generating functions,

$$
\boxed{
G_T(s)=\prod_{r=1}^{n}
\frac{rs}{n-(n-r)s}}.
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [10F](../../10f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

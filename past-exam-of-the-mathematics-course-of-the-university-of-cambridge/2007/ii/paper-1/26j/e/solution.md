<h1 id="26j/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Assign each arriving car independently to a uniformly chosen lot. The [Poisson thinning theorem](../../../../../../poisson-thinning-theorem.md) gives **three independent Poisson processes, each of rate $\lambda/3$**. For an interval of length $t$, their joint [probability generating function](../../../../../../probability-generating-function.md) is

$$
\exp\!\left[\lambda t\left(\frac{z_a+z_b+z_c}{3}-1\right)\right]
=\prod_{i=a,b,c}\exp\left[\frac{\lambda t}{3}(z_i-1)\right].
$$

The factorization proves independence of the counts in that interval; independence over disjoint intervals proves independence of the processes.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [26J](../../26j.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

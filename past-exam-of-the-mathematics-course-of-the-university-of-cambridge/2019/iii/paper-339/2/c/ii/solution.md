<h1 id="2/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

A fixed [edge](../../../../../../../edge-of-a-graph.md) is monochromatic exactly when none of the $r$ hyperplanes separates its endpoints. Each hyperplane fails to cut it with probability at most $1/3$, and the hyperplanes are independent. Therefore

$$
\mathbb P\{c(i)=c(j)\}\leq3^{-r}.
$$

Let $B=\sum_{ij\in E}\mathbf1_{\{c(i)=c(j)\}}$ count monochromatic [edges](../../../../../../../edge-of-a-graph.md). Applying [linearity of expectation](../../../../../../../linearity-of-expectation.md) to these [indicator random variables](../../../../../../../indicator-random-variable.md) gives

$$
\boxed{\mathbb E B\leq m3^{-r}.}
$$

Independence between different [edges](../../../../../../../edge-of-a-graph.md) is unnecessary; only the independently sampled hyperplanes are used. The $r$ signs provide at most $2^r$ colors, whether or not every sign region is nonempty.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [Paper 339](../../../../paper-339-split.md)
5. [Iii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)

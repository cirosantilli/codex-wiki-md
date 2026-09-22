<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $X$ be the number of crossings in the drawing, placed in general position. Deleting at most one edge at each crossing leaves a [planar graph](../../../../../../planar-graph.md), so the [Euler formula for a connected planar graph](../../../../../../euler-formula-for-a-connected-planar-graph.md) gives

$$
m-X\leq3n,
\qquad\text{hence}\qquad X\geq m-3n.
$$

Now retain every vertex independently with probability $p$, together with every edge whose endpoints survive. The expected numbers of retained vertices, edges and crossings are $pn,p^2m,p^4X$. Applying the preceding inequality to each sampled drawing and taking expectations gives

$$
p^4X\geq p^2m-3pn.
$$

Because $m\geq6n$, choose $p=6n/m\leq1$. Then

$$
p^2m-3pn=\frac{18n^2}{m},
$$

and therefore

$$
X\geq\frac{18n^2/m}{(6n/m)^4}
=\frac1{72}\frac{m^3}{n^2}.
$$

**Thus the [Crossing lemma](../../../../../../crossing-lemma.md) holds here with the absolute constant $c=1/72$.**

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 161](../../../paper-161-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

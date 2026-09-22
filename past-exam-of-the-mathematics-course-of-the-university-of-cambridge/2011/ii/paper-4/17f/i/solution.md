<h1 id="17f/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

With one [edge](../../../../../../edge-of-a-graph.md) colour, $f(1)=3$. Suppose the assertion is known for $k-1$ colours, and take $n=k(f(k-1)-1)+2$. At any [vertex](../../../../../../vertex-graph-theory.md), among its $n-1$ incident [edges](../../../../../../edge-of-a-graph.md) some colour occurs on at least $f(k-1)$ [edges](../../../../../../edge-of-a-graph.md). Let $S$ be their other endpoints. If an [edge](../../../../../../edge-of-a-graph.md) within $S$ has that colour, it completes a monochromatic triangle with the chosen [vertex](../../../../../../vertex-graph-theory.md). Otherwise $S$ uses only $k-1$ colours internally, and the inductive hypothesis gives a monochromatic triangle there. Thus

$$
f(k)\le k(f(k-1)-1)+2.
$$

Induction now yields

$$
f(k)\le k(3(k-1)!-1)+2=3k!-k+2\le3k!\qquad(k\ge2).
$$

Together with the base case, **$\boxed{f(k)\le3k!}$ for every positive $k$**. This is a constructive [multicolour Ramsey bound](../../../../../../multicolour-ramsey-bound.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [17F](../../17f.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

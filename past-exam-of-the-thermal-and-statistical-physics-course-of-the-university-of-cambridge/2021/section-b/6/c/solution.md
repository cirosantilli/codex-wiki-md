<h1 id="section-b/6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For this [radial random walk on a regular tree](../../../../../radial-random-walk-on-a-regular-tree.md), the drawing is an infinite [regular tree](../../../../../regular-tree.md) of degree $z$, not a planar lattice with closed loops. The radial coordinate is the number of [edges](../../../../../edge-of-a-graph.md) in the unique path to the root. A non-root [vertex](../../../../../vertex-graph-theory.md) has one neighbour inward and $z-1$ neighbours outward, so equal [probabilities](../../../../../probability.md) for its $z$ [edges](../../../../../edge-of-a-graph.md) give

$$
w_-^{\rm rad}=\frac1z,\qquad w_+^{\rm rad}=\frac{z-1}{z}.
$$

Let $r$ be radial distance measured in [edge](../../../../../edge-of-a-graph.md) units. For $r>1$, [probability](../../../../../probability.md) arriving in shell $r$ comes from shell $r-1$ by an outward step or from shell $r+1$ by an inward step:

$$
\boxed{P(r,N+1)=\frac{z-1}{z}P(r-1,N)+\frac1zP(r+1,N),\qquad r>1.}
$$

This has precisely the same bulk [master equation](../../../../../master-equation.md) as the one-dimensional [biased random walk](../../../../../biased-random-walk.md), with

$$
\boxed{\epsilon=\frac{w_-^{\rm rad}-w_+^{\rm rad}}2=\frac{2-z}{2z}.}
$$

The outward bias is geometric: beyond the first shell, the number of [vertices](../../../../../vertex-graph-theory.md) is $M_r=z(z-1)^{r-1}$, so there are more outward than inward choices even though no [edge](../../../../../edge-of-a-graph.md) direction is dynamically preferred. $P(r,N)$ is the [probability](../../../../../probability.md) summed over an entire shell, not the [probability](../../../../../probability.md) at one specified [vertex](../../../../../vertex-graph-theory.md); no additional shell-size factor belongs in the boxed recurrence.

The equality concerns the evolution equation away from the root, not equality to the unrestricted full-line [binomial distribution](../../../../../binomial-distribution.md) at all positions. The root imposes a different boundary rule.

## ↑ Ancestors (14)

1. [C](../c.md)
2. [6](../../6.md)
3. [Section B](../../../section-b.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the thermal and statistical physics course of the University of Cambridge](../../../../split.md)
6. [Thermal and Statistical Physics course of the University of Cambridge](../../../../../thermal-and-statistical-physics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)

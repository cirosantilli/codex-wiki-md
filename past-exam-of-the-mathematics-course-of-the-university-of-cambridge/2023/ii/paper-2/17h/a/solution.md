<h1 id="17h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a positive integer $t$, the [chromatic polynomial](../../../../../../chromatic-polynomial.md) $P_G(t)$ is defined to be the number of proper [vertex colourings](../../../../../../graph-coloring.md) of $G$ using a fixed palette of $t$ colours.

We prove that this counting function is a polynomial by induction on the number of [edges](../../../../../../edge-of-a-graph.md). If $G$ has $n$ vertices and no edges, every assignment of colours is proper, so

$$
P_G(t)=t^n.
$$

Otherwise choose an edge $e=uv$. Every proper colouring of $G-e$ either gives $u,v$ different colours, in which case it is a colouring of $G$, or gives them the same colour, in which case it corresponds to a proper colouring of the contracted graph $G/e$. Hence the [deletion-contraction recurrence for the chromatic polynomial](../../../../../../deletion-contraction-recurrence-for-the-chromatic-polynomial.md) is

$$
P_G(t)=P_{G-e}(t)-P_{G/e}(t).
$$

Both terms on the right are polynomials by induction, so $P_G$ is a polynomial.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [17H](../../17h.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

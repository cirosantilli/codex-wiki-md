<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [graph Ramsey number](../../../../../../graph-ramsey-number.md) $R(H)$ is the least $N$ such that every red-blue colouring of the edges of $K_N$ contains a monochromatic copy of $H$.

The [minimum-degree Ramsey lower bound](../../../../../../minimum-degree-ramsey-lower-bound.md) states that a graph of [minimum degree](../../../../../../minimum-degree-of-a-graph.md) $d$ admits an $H$-free colouring on every integer $N<2^{d/2}$. Its probabilistic proof colours edges independently and applies the local lemma to the events that a labelled copy of $H$ is monochromatic. Since

$$
e(H)\geq\frac{d|V(H)|}{2},
$$

the exponential cost $2^{1-e(H)}$ of a monochromatic copy dominates the number of compatible copies through every fixed edge. Hence such a colouring exists, and therefore

$$
\boxed{R(H)\geq2^{d/2}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 122](../../../paper-122-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

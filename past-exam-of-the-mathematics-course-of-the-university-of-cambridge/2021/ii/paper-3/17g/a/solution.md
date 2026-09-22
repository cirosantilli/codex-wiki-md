<h1 id="17g/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The diagonal [Ramsey number](../../../../../../diagonal-ramsey-number.md) $R(k)$ is the least $n$ such that every red-blue coloring of $K_n$ contains a monochromatic $K_k$. The standard recursion

$$
R(s,t)\leq R(s-1,t)+R(s,t-1)
$$

gives

$$
R(k)\leq\binom{2k-2}{k-1}<4^k.
$$

Thus the converted $k^4$ is a superscript-order error; that bound is false for large $k$.

In a red-blue coloring, if the red spanning graph is connected it has a red spanning tree. Otherwise its red components are joined pairwise by blue edges, making the blue graph connected, so it has a blue spanning tree.

The result fails for three colors. Color the six edges of $K_4$ by its three perfect matchings, one color per matching. Every monochromatic graph then consists of two disjoint edges and has no spanning tree.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [17G](../../17g.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

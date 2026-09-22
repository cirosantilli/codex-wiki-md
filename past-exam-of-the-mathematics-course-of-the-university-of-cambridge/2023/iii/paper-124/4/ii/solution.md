<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

View $M$ as a directed graph with nonnegative integer edge weights. For an edge of weight

$$
w=\sum_{j=0}^{n-1}b_j2^j,
\qquad b_j\in\{0,1\},
$$

build a [binary path-counting gadget](../../../../../../binary-path-counting-gadget.md) with one entrance and one exit and exactly $w$ entrance-to-exit routes. Starting with one route, a constant-size diamond doubles the number of routes; processing the bits from most significant to least significant repeatedly doubles and, when $b_j=1$, adds one bypass route. The gadget has $O(n)$ vertices and only zero-one edges.

Add forced internal edges and self-loops so that a cycle cover not using the simulated edge extends uniquely across the gadget, whereas a cycle cover using it has exactly one extension for each entrance-to-exit route. Replacing every weighted edge therefore multiplies each original cycle cover by precisely the product of its selected edge weights. Summing over covers gives

$$
\operatorname{perm}N=\operatorname{perm}M.
$$

There are $n^2$ entries and each gadget has $O(n)$ size, so $N$ is constructed in polynomial time.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 124](../../../paper-124-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

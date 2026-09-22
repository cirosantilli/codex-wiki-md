<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Couple two configurations differing at one vertex $u$ by choosing the same update vertex and the same uniform random number for the heat-bath update. Updating $u$ removes the disagreement. Updating a nonneighbor of $u$ cannot create one. At a neighbor $v$, the two conditional plus-spin probabilities differ by at most $\tanh\beta$, using the supplied identity. Since $u$ has at most $\Delta$ neighbors, the expected Hamming distance after one step is at most

$$
1-\frac1n+\frac{\Delta\tanh\beta}{n}
=1-\frac{1-\Delta\tanh\beta}{n}.
$$

The Hamming diameter is $n$, so the [Path coupling theorem](../../../../../../path-coupling-theorem.md) gives

$$
\boxed{d(t)\leq n\left(1-\frac{1-\Delta\tanh\beta}{n}\right)^t.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 215](../../../paper-215-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

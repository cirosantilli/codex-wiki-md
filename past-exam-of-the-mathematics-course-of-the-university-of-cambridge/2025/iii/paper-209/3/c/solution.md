<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The conditional open probability in part (b) is increasing in the states of all other edges, because adding edges can only connect the two endpoints. A common-uniform update therefore preserves the coordinatewise order. Start two copies from all closed and use the same updates, with the second copy additionally conditioned through an increasing event $B$ by the corresponding monotone censored heat-bath chain. The monotone grand coupling and convergence to stationarity show that conditioning on $B$ stochastically increases the configuration. Hence for increasing $A$,

$$
\phi_{p,2}(A\mid B)\geq\phi_{p,2}(A),
$$

which is the [Harris-FKG inequality](../../../../../../harris-fkg-inequality.md) $\phi(A\cap B)\geq\phi(A)\phi(B)$. Applying this to the complement of a decreasing event $B'$ gives

$$
\boxed{\phi(A\cap B')\leq\phi(A)\phi(B').}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 209](../../../paper-209-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The chain rule, now separating $X_i$ first, gives

$$
D(Q\Vert P)
=D(Q_{X_i}\Vert P_{X_i})
+D(Q_{X^{(i)}\mid X_i}\Vert P_{X^{(i)}}\mid Q_{X_i}),
$$

where the second term denotes the conditional divergence averaged over $Q_{X_i}$. Summing over $i$ yields

$$
\sum_iD(Q_{X^{(i)}\mid X_i}\Vert P_{X^{(i)}}\mid Q_{X_i})
=nD(Q\Vert P)-\sum_iD(Q_{X_i}\Vert P_{X_i}).
$$

Repeated use of the chain rule and convexity gives the [tensorization lower bound for relative entropy](../../../../../../tensorization-lower-bound-for-relative-entropy.md)

$$
\sum_iD(Q_{X_i}\Vert P_{X_i})\leq D(Q\Vert P).
$$

**Therefore the preceding sum is at least $(n-1)D(Q\Vert P)$, which is equivalent to the required inequality.**

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 208](../../../paper-208-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

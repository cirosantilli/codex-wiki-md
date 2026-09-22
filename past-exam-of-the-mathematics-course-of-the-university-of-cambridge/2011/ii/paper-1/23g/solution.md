<h1 id="23g/solution">Solution</h1>

↑ **Parent:** [23G](../23g.md)

Near an isolated point $P\in A$, choose source and target coordinate charts, using continuity of $\alpha$ to keep a sufficiently small source neighbourhood in the target chart. The coordinate representation is holomorphic on the punctured neighbourhood and is bounded near $P$ by continuity. The [Riemann removable singularity theorem](../../../../../riemann-removable-singularity-theorem.md) extends it holomorphically across $P$, with the given continuous value. Repeating at all points of $A$ proves that **$\alpha$ is analytic**.

For a nonconstant holomorphic function $f$ on a connected [Riemann surface](../../../../../riemann-surfaces.md), let $A$ be the set where its coordinate derivative vanishes. This condition is independent of the chart. The derivative cannot vanish identically on an open set, because the [identity theorem](../../../../../identity-theorem.md) would then make $f$ constant globally. Its zeros are isolated and closed locally, so $A$ is a closed discrete subset. At every other point the [holomorphic inverse function theorem](../../../../../holomorphic-inverse-function-theorem.md) makes $f$ a local coordinate chart.

Now suppose $\alpha$ is a homeomorphism and $g=f\circ\alpha$ is analytic. Outside $\alpha^{-1}(A)$, use $f$ as a target coordinate to write locally $\alpha=f^{-1}\circ g$. This is analytic. The preimage $\alpha^{-1}(A)$ is discrete because $\alpha$ is a homeomorphism, and the first argument extends analyticity across it. An injective holomorphic map cannot have a zero derivative: a zero of order at least two would give a locally multiple-to-one map. Its local inverse is therefore holomorphic, proving that **$\alpha$ is a conformal equivalence**.

The plane $\mathbb C$ and the unit disk are homeomorphic by $z\mapsto z/(1+|z|)$, with inverse $w\mapsto w/(1-|w|)$. They are not conformally equivalent: a holomorphic equivalence from the plane to the disk would be a bounded nonconstant [entire function](../../../../../entire-function.md), contradicting [Liouville's theorem](../../../../../liouville-theorem.md).

## ↑ Ancestors (11)

1. [23G](../23g.md)
2. [Section II](../section-ii.md)
3. [Paper 1](../../paper-1-split.md)
4. [Ii](../../split.md)
5. [2011](../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)

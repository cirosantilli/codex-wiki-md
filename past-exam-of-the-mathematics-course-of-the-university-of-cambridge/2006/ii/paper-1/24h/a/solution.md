<h1 id="24h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [manifold](../../../../../../topological-manifold.md) [inverse function theorem](../../../../../../inverse-function-theorem.md) states: if $f:X\to Y$ is smooth and $df_x:T_xX\to T_{f(x)}Y$ is an isomorphism, there are open neighborhoods $U$ of $x$ and $V$ of $f(x)$ such that $f:U\to V$ is a [diffeomorphism](../../../../../../diffeomorphism.md). In particular the [manifolds](../../../../../../topological-manifold.md) have the same dimension at those points.

Choose charts $\phi$ around $x$ and $\psi$ around $f(x)$, shrinking the source chart so its image under $f$ lies in the target chart. The coordinate map $F=\psi\circ f\circ\phi^{-1}$ has [derivative](../../../../../../derivative.md) $d\psi\circ df_x\circ d\phi^{-1}$, an invertible [matrix](../../../../../../matrix.md). Apply the permitted Euclidean [inverse function theorem](../../../../../../inverse-function-theorem.md) to obtain open coordinate neighborhoods on which $F$ and $F^{-1}$ are smooth. Pull them back through the charts. The resulting inverse is $\phi^{-1}\circ F^{-1}\circ\psi$, smooth by composition. This proves the [manifold](../../../../../../topological-manifold.md) statement.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [24H](../../24h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

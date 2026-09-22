<h1 id="37d/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write

$$
J^\alpha{}_{\mu}=\frac{\partial\widetilde x^\alpha}{\partial x^\mu}.
$$

By the [chain rule](../../../../../../../chain-rule.md), $\widetilde V^\alpha=J^\alpha{}_{\mu}V^\mu$, $\widetilde W^\alpha=J^\alpha{}_{\mu}W^\mu$, and $\widetilde V^\beta\widetilde\partial_\beta=V^\nu\partial_\nu$. Therefore

$$
\begin{aligned}
[\widetilde V,\widetilde W]^\alpha
&=V^\nu\partial_\nu(J^\alpha{}_{\mu}W^\mu)-W^\nu\partial_\nu(J^\alpha{}_{\mu}V^\mu)\\
&=J^\alpha{}_{\mu}[V,W]^\mu+(V^\nu W^\mu-W^\nu V^\mu)\frac{\partial^2\widetilde x^\alpha}{\partial x^\nu\partial x^\mu}.
\end{aligned}
$$

The last term vanishes because its first factor is antisymmetric in $\mu,\nu$ and its second is symmetric. Thus the [coordinate invariance of the Lie bracket](../../../../../../../coordinate-invariance-of-the-lie-bracket.md) is

$$
\boxed{[\widetilde V,\widetilde W]^\alpha=J^\alpha{}_{\mu}[V,W]^\mu.}
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [37D](../../../37d.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [Ii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)

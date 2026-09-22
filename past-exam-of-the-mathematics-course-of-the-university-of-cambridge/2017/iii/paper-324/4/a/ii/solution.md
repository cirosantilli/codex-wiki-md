<h1 id="4/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Label the measured [vertex](../../../../../../../vertex-graph-theory.md) of the four-cycle by $0$, its two neighbours by $1,3$, and the opposite [vertex](../../../../../../../vertex-graph-theory.md) by $2$. The [edges](../../../../../../../edge-of-a-graph.md) are $01,12,23,30$. By the definition of a [graph state](../../../../../../../graph-state.md),

$$
|\psi_{2\times2}\rangle=E_{01}E_{12}E_{23}E_{30}|+\rangle^{\otimes4}.
$$

All [Controlled-Z gates](../../../../../../../controlled-z-gate.md) commute. Conditioning on the [computational basis](../../../../../../../computational-basis.md) value $r$ of [vertex](../../../../../../../vertex-graph-theory.md) $0$, the factors on [edges](../../../../../../../edge-of-a-graph.md) $01$ and $03$ act on their other endpoints as $Z_1^r$ and $Z_3^r$, since $E|r,a\rangle=(-1)^{ra}|r,a\rangle$. The remaining [edges](../../../../../../../edge-of-a-graph.md) form the three-[vertex](../../../../../../../vertex-graph-theory.md) path $1-2-3$:

$$
{}_0\langle r|\psi_{2\times2}\rangle=\frac1{\sqrt2}Z_1^rZ_3^rE_{12}E_{23}|+\rangle_1|+\rangle_2|+\rangle_3.
$$

The [Born rule](../../../../../../../born-rule.md) gives probability one half for either result. Normalizing proves

$$
\boxed{|\psi_{\mathrm{remaining}}\rangle=(Z^r\otimes I\otimes Z^r)|\psi_3\rangle.}
$$

This is [computational-basis measurement of a graph-state vertex](../../../../../../../computational-basis-measurement-of-a-graph-state-vertex.md): remove the measured [vertex](../../../../../../../vertex-graph-theory.md) and apply a known [Pauli Z gate](../../../../../../../pauli-z-gate.md) byproduct to each neighbour. The chosen labels specify precisely which factors occur; any [vertex](../../../../../../../vertex-graph-theory.md) of the square can serve as [vertex](../../../../../../../vertex-graph-theory.md) $0$ by relabelling.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [4](../../../4.md)
4. [Paper 324](../../../../paper-324-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)

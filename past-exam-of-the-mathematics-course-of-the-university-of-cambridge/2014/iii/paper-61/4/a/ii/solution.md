<h1 id="4/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

An explicit [measurement-based quantum computation](../../../../../../../measurement-based-quantum-computation.md) pattern uses six vertices $u_0,u_1,u_2,v_0,v_1,v_2$. Prepare a [graph state](../../../../../../../graph-state.md) with every vertex in $|+\rangle$ and apply a [Controlled-Z gate](../../../../../../../controlled-z-gate.md) for each edge

$$
(u_0,u_1),\ (u_1,u_2),\ (v_0,v_1),\ (v_1,v_2),\ (u_2,v_1).
$$

The first two links on each wire permit [graph-state preparation of a computational-basis input](../../../../../../../graph-state-preparation-of-a-computational-basis-input.md) followed by the logical [J gate](../../../../../../../j-gate-in-measurement-based-quantum-computation.md). Use the following single-qubit measurements:

- Measure $u_0$ and $v_0$ in the $X$ basis, obtaining $s_0,t_0$.
- Measure $u_1$ in the equatorial basis with angle $(-1)^{s_0}\alpha$, obtaining $s_1$.
- Measure $v_1$ in the equatorial basis with angle $(-1)^{t_0}\beta$, obtaining $t_1$.
- Measure $v_2$ in the $Z$ basis, obtaining $m$, and return $b_2=m\oplus s_1\oplus t_1$. The unmeasured $u_2$ can be discarded.

All entangling edges can be made at preparation time because [Controlled-Z gates](../../../../../../../controlled-z-gate.md) commute. A future edge that does not touch a currently measured vertex can equivalently be deferred, which allows the [one-bit teleportation](../../../../../../../one-bit-teleportation.md) identities to be applied in their logical order.

The two initial $X$ measurements implement $H|+\rangle=|0\rangle$ with [Pauli frames](../../../../../../../pauli-frame.md) $X^{s_0},X^{t_0}$ on the logical inputs. The first adaptive [J gate](../../../../../../../j-gate-in-measurement-based-quantum-computation.md) then has output frame $X^{s_1}Z^{s_0}$ on $u_2$. Propagating through $E_{u_2v_1}$ gives frames

$$
X^{s_1}Z^{s_0\oplus t_0}\ \text{on }u_2,
\qquad X^{t_0}Z^{s_1}\ \text{on }v_1,
$$

up to branchwise global phase. The second adaptive [J gate](../../../../../../../j-gate-in-measurement-based-quantum-computation.md) converts the latter into

$$
X^{t_1\oplus s_1}Z^{t_0}\ \text{on }v_2.
$$

A $Z$ correction does not alter a computational-basis measurement, while an $X$ correction flips its bit. Consequently the deterministic classical postprocessing is

$$
\boxed{b_2=m\oplus s_1\oplus t_1}.
$$

This reproduces the output-bit distribution of the original [quantum circuit](../../../../../../../quantum-circuit-split.md), including its known byproduct corrections.

<a id="4/a/ii/image-six-vertex-graph-state-adaptive-equatorial-measurements-and-classical-parity-correction-for-the-two-wire-circuit"></a>
![](../../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-61-measurement-pattern.png)

**[Figure 1](#4/a/ii/image-six-vertex-graph-state-adaptive-equatorial-measurements-and-classical-parity-correction-for-the-two-wire-circuit). Six-vertex graph state, adaptive equatorial measurements and classical parity correction for the two-wire circuit**.

There is an additional simplification for these particular zero inputs. Since $J(\alpha)|0\rangle=|+\rangle$, $E(|+\rangle|0\rangle)=|+\rangle|0\rangle$, and $J(\beta)|0\rangle=|+\rangle$, the exact final state is $|+\rangle|+\rangle$, independently of the angles. The requested bit is therefore fair. A single isolated graph-state vertex measured in $Z$ already simulates that bit distribution; the six-vertex pattern also explicitly realizes the circuit and its corrections.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [4](../../../4.md)
4. [Paper 61](../../../../paper-61-split.md)
5. [Iii](../../../../split.md)
6. [2014](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)

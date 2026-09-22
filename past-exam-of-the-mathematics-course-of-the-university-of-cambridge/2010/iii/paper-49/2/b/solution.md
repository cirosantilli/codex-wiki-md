<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Prepare the [three-vertex graph-state wire](../../../../../../three-vertex-graph-state-wire.md): start all three [qubits](../../../../../../qubit.md) in $|+\rangle$ and apply [Controlled-Z gates](../../../../../../controlled-z-gate.md) on edges $1-2$ and $2-3$. In this paper's [equatorial qubit measurement](../../../../../../equatorial-qubit-measurement.md) convention the basis vectors can be chosen as

$$
|v_r(\theta)\rangle=\frac{|0\rangle+(-1)^re^{i\theta}|1\rangle}{\sqrt2}.
$$

The given identity means that measuring an input qubit at angle $\theta$, with outcome $r$, teleports its state to the next qubit as $X^rU(\theta)|\psi\rangle$. Each outcome has probability $1/2$, since $X^rU(\theta)$ is unitary. This is [one-bit teleportation](../../../../../../one-bit-teleportation.md) with a known [Pauli frame](../../../../../../pauli-frame.md).

Measure vertex 1 at angle $\alpha$ and record $r$. Then measure vertex 2 at angle $\gamma=(-1)^r\beta$, taken modulo $2\pi$, and record $s$. The controlled-Z on edge $2-3$ commutes with the first measurement, so the two teleportation steps can be applied successively. The remaining normalized state is

$$
X^sU(\gamma)X^rU(\alpha)|+\rangle.
$$

For $r=0$ this is $X^sU(\beta)U(\alpha)|+\rangle$. For $r=1$, the relation proved above gives $U(-\beta)X=e^{i\beta}ZU(\beta)$. Thus in every branch the remaining state is

$$
e^{ir\beta}X^sZ^rU(\beta)U(\alpha)|+\rangle.
$$

The scalar is a [global phase](../../../../../../global-phase.md) and has no effect on probabilities.

Finally measure vertex 3 in the [computational basis](../../../../../../computational-basis.md), obtaining $z$, and report

$$
\boxed{k=z\oplus s.}
$$

The $Z^r$ byproduct changes only computational-basis phases; $X^s$ changes the output label by $s$. Hence the corrected bit has exactly the ideal circuit's [probability distribution](../../../../../../probability-distribution.md) in every branch, not merely on average. The procedure uses only single-qubit measurements after preparing the graph state, adaptive classical angle selection, and deterministic classical output processing.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 49](../../../paper-49-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

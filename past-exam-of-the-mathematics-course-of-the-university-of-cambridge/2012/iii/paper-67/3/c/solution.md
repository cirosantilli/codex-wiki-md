<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write the single-qubit gate as $R(\alpha)=HP(\alpha)H$, where $P(\alpha)=\operatorname{diag}(1,e^{i\alpha})$. Thus it is, up to [global phase](../../../../../../global-phase.md), a [rotation about the x-axis](../../../../../../rotation-about-the-x-axis.md), and it commutes with $X$. Compile it as a [Hadamard gate](../../../../../../hadamard-gate.md) followed by the [J gate](../../../../../../j-gate-in-measurement-based-quantum-computation.md) $J(\alpha)$. Compile each [CNOT gate](../../../../../../controlled-not-gate.md) as before into $H_jE_{ij}H_j$. The usual wire-link construction yields a resource [graph state](../../../../../../graph-state.md) for the fixed $|+\rangle$ inputs; the same frame algebra also works for logical input states supplied to an open resource.

The point is stronger than counting two gates per rotation: a long circuit must not acquire a new adaptive layer for every rotation. We show that every nonzero-angle basis depends only on outcomes of the angle-zero measurements.

For an $R(\alpha)$ gadget, let the incoming [Pauli frame](../../../../../../pauli-frame.md) be $X^pZ^q$. Denote the angle-zero outcome by $s$, and the subsequent angle-$\theta$ outcome by $t$. The two [one-bit teleportations](../../../../../../one-bit-teleportation.md) give

$$
X^tJ(\theta)X^sHX^pZ^q\simeq X^{t\oplus p}Z^{s\oplus q}R(\alpha),\qquad \theta=(-1)^{s\oplus q}\alpha,
$$

where $\simeq$ omits a [global phase](../../../../../../global-phase.md). Consequently the rotation gadget updates

$$
\boxed{p'=p\oplus t,\qquad q'=q\oplus s.}
$$

Only its angle-zero outcome enters the new $Z$ frame. Its arbitrary-angle outcome enters only the $X$ frame, which commutes through all later $R$ gates.

For a [CNOT gate](../../../../../../controlled-not-gate.md) from $i$ to $j$, call the outcomes of its two angle-zero target-wire measurements $r,u$, in that order. The [Pauli frame](../../../../../../pauli-frame.md) update is

$$
p_i'=p_i,\qquad p_j'=p_j\oplus p_i\oplus u,\qquad q_i'=q_i\oplus q_j\oplus r,\qquad q_j'=q_j\oplus r.
$$

These follow by applying the preceding [Hadamard gate](../../../../../../hadamard-gate.md) and [Controlled-Z gate](../../../../../../controlled-z-gate.md) frame updates twice. In particular, the new $Z$ frames depend on old $Z$ frames and angle-zero outcomes only; they never depend on old $X$ frames or arbitrary-angle outcomes. This is the measurement-level version of the given fact that a [CNOT gate](../../../../../../controlled-not-gate.md) propagates $X$ operators into products of $X$ operators.

Starting with no frame, induction in the original circuit order now computes every $q$ solely from angle-zero results. Therefore every sign $(-1)^{s\oplus q}$ is known after one simultaneous layer containing **all angle-zero measurements**, including those appearing late in the circuit. Compute those signs classically, and perform **all remaining equatorial measurements in a second simultaneous layer**. An angle zero that occurs accidentally among these remaining choices may stay in that layer. Reordering is valid because, once a branch's bases have been fixed, the projectors on different vertices commute; no second-layer result is needed to choose another second-layer basis.

The [two-layer measurement pattern for CNOT and x-axis rotations](../../../../../../two-layer-measurement-pattern-for-cnot-and-x-axis-rotations.md) thus has

$$
\boxed{\text{logical measurement depth}\le2,}
$$

independently of the number or order of gates. Fixed [computational-basis measurements](../../../../../../quantum-measurement-in-the-computational-basis.md) of classical outputs can be included in layer two, followed by relabelling $t_i\mapsto t_i\oplus p_i$. For quantum outputs the final [Pauli frame](../../../../../../pauli-frame.md) gives the required correction. The depth statement excludes graph preparation and classical processing, as in the definition in the paper.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

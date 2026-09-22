<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Label the chain [cluster state](../../../../../../cluster-state.md) from top to bottom by $1,2,3,4$, and let $k,l,m$ be the phase-measurement outcomes on the first three vertices, with raw [computational basis](../../../../../../computational-basis.md) outcome $s$ on vertex four. Repeated [one-bit teleportation](../../../../../../one-bit-teleportation.md) leaves the last [qubit](../../../../../../qubit.md), up to [global phase](../../../../../../global-phase.md), in

$$
|\chi\rangle=X^mU(\gamma)X^lU(\beta)X^kU(\alpha)|+\rangle.
$$

This sequential description applies even though the whole [graph state](../../../../../../graph-state.md) is prepared first: a later [Controlled-Z gate](../../../../../../controlled-z-gate.md) acts only on unmeasured [qubits](../../../../../../qubit.md) and commutes with earlier single-[qubit](../../../../../../qubit.md) measurement operators. It can therefore be moved past those measurements for the purpose of calculating each conditional branch.

Take $\alpha=\theta$ and $\beta=0$, so $U(0)=H$. After the second measurement the logical state is

$$
X^lHX^kU(\theta)|+\rangle=X^lZ^kHU(\theta)|+\rangle.
$$

For binary $p,q$, the identities proved above imply the [Pauli-frame propagation along a measurement wire](../../../../../../pauli-frame-propagation-along-a-measurement-wire.md) rule

$$
U(\eta)X^pZ^q\simeq X^qZ^pU((-1)^p\eta),
$$

where $\simeq$ means equality up to [global phase](../../../../../../global-phase.md). Choose the third angle adaptively as $\gamma=(-1)^{l\oplus1}\phi$. Then $(-1)^l\gamma=-\phi$, and

$$
|\chi\rangle\simeq X^{m\oplus k}Z^lU(-\phi)HU(\theta)|+\rangle.
$$

Reading the target circuit in temporal order gives its premeasurement state

$$
|T\rangle=U(\phi)XHU(\theta)H|0\rangle
=e^{-i\phi}ZU(-\phi)HU(\theta)|+\rangle.
$$

Consequently

$$
|\chi\rangle\simeq X^{m\oplus k}Z^{l\oplus1}|T\rangle.
$$

The [Pauli Z gate](../../../../../../pauli-z-gate.md) changes only phases in the [computational basis](../../../../../../computational-basis.md), while the [Pauli X gate](../../../../../../pauli-x-gate.md) exchanges its two measurement outcomes. Thus the explicit choices are

$$
\boxed{\alpha=\theta,\quad\beta=0,\quad\gamma=(-1)^{l\oplus1}\phi,\quad\delta=k\oplus m,\quad r=s\oplus k\oplus m.}
$$

Indeed, for every earlier outcome branch,

$$
\Pr(r=t\mid k,l,m)=|\langle t|T\rangle|^2\qquad(t=0,1).
$$

Hence averaging over the earlier random outcomes leaves exactly the target [probability distribution](../../../../../../probability-distribution.md). This implements the desired [measurement-based quantum computation](../../../../../../measurement-based-quantum-computation.md) without physically removing the final [Pauli frame](../../../../../../pauli-frame.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 51](../../../paper-51-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

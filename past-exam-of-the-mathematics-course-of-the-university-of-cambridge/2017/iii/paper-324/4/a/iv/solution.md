<h1 id="4/a/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Let the ideal two-[qubit](../../../../../../../qubit.md) output before final [measurement in quantum measurements](../../../../../../../quantum-measurement-split.md) be

$$
|\Omega\rangle=E_{23}J(\alpha)_2|+\rangle_2|+\rangle_3.
$$

The PDF places $J(\alpha)$ only on the upper wire, followed by the [Controlled-Z gate](../../../../../../../controlled-z-gate.md) and a [quantum measurement in the computational basis](../../../../../../../quantum-measurement-in-the-computational-basis.md) on each output wire. Measure [vertex](../../../../../../../vertex-graph-theory.md) $0$ of the square in the [computational basis](../../../../../../../computational-basis.md), obtaining $r$, then [vertex](../../../../../../../vertex-graph-theory.md) $1$ of the surviving path in the fixed [equatorial qubit measurement](../../../../../../../equatorial-qubit-measurement.md) basis at angle $\alpha$, obtaining $s$. Put $t=r\oplus s$. The previous part gives $E_{23}X_2^tJ(\alpha)_2Z_3^r|++\rangle$.

Commute its [Pauli frame](../../../../../../../pauli-frame.md) through the [Controlled-Z gate](../../../../../../../controlled-z-gate.md). Since $E_{23}X_2^t=X_2^tZ_3^tE_{23}$ and $E_{23}$ commutes with $Z_3^r$, the actual output is

$$
X_2^{r\oplus s}Z_3^s|\Omega\rangle.
$$

Finally measure [vertices](../../../../../../../vertex-graph-theory.md) $2,3$ in the [computational basis](../../../../../../../computational-basis.md), with raw results $d_2,d_3$. A [Pauli X gate](../../../../../../../pauli-x-gate.md) flips a [computational basis](../../../../../../../computational-basis.md) result, whereas a [Pauli Z gate](../../../../../../../pauli-z-gate.md) changes only its phase. Thus the purely classical correction is

$$
\boxed{k=d_2\oplus r\oplus s,\qquad l=d_3.}
$$

This [four-cycle graph-state simulation of an entangle-and-measure circuit](../../../../../../../four-cycle-graph-state-simulation-of-an-entangle-and-measure-circuit.md) reproduces the full joint output distribution, not just each marginal. All measurement bases are fixed beforehand, and no physical byproduct correction is necessary. As a check, the ideal [Controlled-Z gate](../../../../../../../controlled-z-gate.md) is diagonal in the output basis, so $P(k,l)=\tfrac12\cos^2(\alpha/2)$ for $k=0$ and $\tfrac12\sin^2(\alpha/2)$ for $k=1$, independently of $l$. The measurement procedure gives exactly these probabilities after its classical relabelling.

## ↑ Ancestors (12)

1. [Iv](../iv.md)
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

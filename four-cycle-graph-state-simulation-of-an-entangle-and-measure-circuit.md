# Four-cycle graph-state simulation of an entangle-and-measure circuit

↑ **Parent:** [Measurement-based quantum computation](measurement-based-quantum-computation.md)

Label a four-cycle $0-1-2-3-0$. Measure [vertex](vertex-graph-theory.md) $0$ in the [computational basis](computational-basis.md) with result $r$, then [vertex](vertex-graph-theory.md) $1$ in the [equatorial qubit measurement](equatorial-qubit-measurement.md) basis at angle $\alpha$ with result $s$. [Graph-state vertex deletion](computational-basis-measurement-of-a-graph-state-vertex.md) and [one-bit teleportation](one-bit-teleportation.md) leave

$$
E_{23}X_2^{r\oplus s}J(\alpha)_2Z_3^r|++\rangle=X_2^{r\oplus s}Z_3^sE_{23}J(\alpha)_2|++\rangle.
$$

Final [computational basis](computational-basis.md) measurements with raw results $d_2,d_3$ therefore simulate the ideal circuit $E_{23}J(\alpha)_2$ on $|++\rangle$ after the classical correction $k=d_2\oplus r\oplus s$, $l=d_3$. The output [probability distribution](probability-distribution.md) is correct in every prior branch; no physical [Pauli frame](pauli-frame.md) correction is needed.

## ↑ Ancestors (6)

1. [Measurement-based quantum computation](measurement-based-quantum-computation.md)
2. [Quantum circuit](quantum-circuit-split.md)
3. [Quantum theory](quantum-theory-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-324/4/a/iv/solution.md)

# Binary-angle implementation of a quantum variable rotation

↑ **Parent:** [Quantum variable rotation](quantum-variable-rotation.md)

Suppose a [reversible circuit](reversible-circuit.md) computes the angle bits $b_l(x)$ in $\theta_x=\sum_l b_l(x)\alpha_l$, where $\alpha_l$ are known binary place values. Apply a [controlled unitary gate](controlled-unitary-gate.md) $R_y(2\alpha_l)$ to the target for each set angle bit. The [rotations about the y-axis](rotation-about-the-y-axis.md) commute and their angles add, giving $R_y(2\theta_x)$. Finally perform [uncomputation](uncomputation.md) of the angle and arithmetic workspace. An $L$-bit angle needs $L$ controlled rotations and twice the reversible angle-computation cost. This preserves coherent superpositions of inputs and underlies the [HHL controlled reciprocal rotation](hhl-controlled-reciprocal-rotation.md).

## ↑ Ancestors (6)

1. [Quantum variable rotation](quantum-variable-rotation.md)
2. [Controlled unitary gate](controlled-unitary-gate.md)
3. [Quantum theory](quantum-theory-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-324/4/b/solution.md)
- [Rotation about the y-axis](rotation-about-the-y-axis.md)

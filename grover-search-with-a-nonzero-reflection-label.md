# Grover search with a nonzero reflection label

↑ **Parent:** [Grover's algorithm](grover-s-algorithm.md)

Let $|s\rangle=H^{\otimes n}|0^n\rangle$, let $U_f$ be the [marked-state phase oracle](marked-state-phase-oracle.md), and replace reflection about $|0^n\rangle$ by reflection about a known [computational basis](computational-basis.md) vector $|y\rangle$. Define $T_y=\bigotimes_{j=0}^{n-1}Z_j^{y_j}$, so $T_y|x\rangle=(-1)^{x\cdot y}|x\rangle$ and $H^{\otimes n}|y\rangle=T_y|s\rangle$. The resulting Grover iterate obeys

$$
G_y=(2|s_y\rangle\langle s_y|-I)U_f=T_yGT_y,\qquad |s_y\rangle=T_y|s\rangle,
$$

because the two diagonal operators $T_y,U_f$ commute. Thus the good and bad uniform vectors are replaced by their signed vectors $T_y|g\rangle,T_y|b\rangle$, with exactly the same [Grover rotation angle](grover-rotation-angle.md). Initializing in $H^{\otimes n}|y\rangle$ gives $G_y^r|s_y\rangle=T_yG^r|s\rangle$. Computational-basis measurement probabilities are unchanged because $T_y$ only multiplies amplitudes by signs.

## ↑ Ancestors (5)

1. [Grover's algorithm](grover-s-algorithm.md)
2. [Quantum theory](quantum-theory-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-57/2/c/solution.md)

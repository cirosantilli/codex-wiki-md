# Optimal three-to-one qubit random access code

↑ **Parent:** [Quantum random access code](quantum-random-access-code.md)

Encode signs $s_j=(-1)^{b_j}$ by the unit [Bloch vector](bloch-vector.md) $(s_1,s_2,s_3)/\sqrt3$. Perform the requested [Pauli measurement](measurement-of-a-pauli-observable.md) and interpret a positive outcome as zero. Every input and index has success $p_*$. To prove optimality, write each binary-measurement difference as $D_j=t_jI+v_j\cdot\sigma$, where positivity gives $|v_j|\le1-|t_j|$. Averaging over all eight inputs cancels the $t_j$ terms. For any encoding vectors of norm at most one, the average success is at most $1/2+(1/48)\sum_s|\sum_js_jv_j|$. The [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md) bounds the sum by $8\sqrt{\sum_j|v_j|^2}\le8\sqrt3$, proving the optimum even for mixed encodings and general binary measurements. The constant-success construction also maximizes worst-case success.

## ↑ Ancestors (6)

1. [Quantum random access code](quantum-random-access-code.md)
2. [Quantum information theory](quantum-information-theory-split.md)
3. [Quantum theory](quantum-theory-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-58/3/e/solution.md)

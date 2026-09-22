<h1 id="1/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Use $|1\rangle$ as the target register for [quantum phase estimation](../../../../../../../quantum-phase-estimation.md) of $U_a$. By part (iii), it is the equal superposition $r^{-1/2}\sum_s|\psi_s\rangle$ of eigenvectors with phases $s/r$. Controlled modular multiplications implement the required powers $U_a^{2^j}$ efficiently. The phase-estimation circuit produces

$$
\frac1{\sqrt r}\sum_{s=0}^{r-1}
|\widetilde{s/r}\rangle|\psi_s\rangle,
$$

where the first register contains an $m$-bit approximation with constant success probability. A [quantum measurement in the computational basis](../../../../../../../quantum-measurement-in-the-computational-basis.md) therefore outputs an approximation to $s/r$, with $s$ uniformly distributed over $\{0,\ldots,r-1\}$.

## ↑ Ancestors (12)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 324](../../../../paper-324-split.md)
5. [Iii](../../../../split.md)
6. [2025](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)

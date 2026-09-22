<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Put $p=\langle\psi|M_1^2|\psi\rangle\geq1-\varepsilon$. Since $M_1$ is a [positive contraction](../../../../../../positive-contraction.md), the successful [post-measurement state](../../../../../../post-measurement-state.md) is the pure state represented by $|\psi'\rangle=M_1|\psi\rangle/\sqrt p$. Its squared [quantum fidelity](../../../../../../fidelity-of-quantum-states.md) with the input is

$$
F(\rho,\rho')^2=|\langle\psi|\psi'\rangle|^2
=\frac{\langle\psi|M_1|\psi\rangle^2}{p}.
$$

The [finite-dimensional spectral theorem](../../../../../../finite-dimensional-spectral-theorem.md) and $0\leq M_1\leq I$ give $M_1^2\leq M_1$, so $\langle M_1\rangle\geq p$. Therefore the [pure-state gentle measurement bound](../../../../../../pure-state-gentle-measurement-bound.md) is

$$
\boxed{F(\rho,\rho')^2\geq p\geq1-\varepsilon}.
$$

The positive-operator assumption matters: an arbitrary unitary measurement operator can have success probability one while rotating the state to an orthogonal vector.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 323](../../../paper-323-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

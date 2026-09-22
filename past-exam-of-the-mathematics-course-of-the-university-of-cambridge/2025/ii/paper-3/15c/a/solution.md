<h1 id="15c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\rho_j=|\alpha_j\rangle\langle\alpha_j|$. For a two-outcome measurement with effect $0\leq M\leq I$ interpreted as guess zero,

$$
P_s=\frac12\operatorname{tr}(M\rho_0)
\frac12\operatorname{tr}((I-M)\rho_1)
=\frac12+\frac12\operatorname{tr}[M(\rho_0-\rho_1)].
$$

The positive-eigenspace projector of $\rho_0-\rho_1$ maximizes the last trace, giving the Helstrom formula

$$
P_s^{\rm opt}=\frac12+\frac14\|\rho_0-\rho_1\|_1.
$$

On the span of the two states, $\rho_0-\rho_1$ has eigenvalues

$$
\mathord\pm\sqrt{1-|\langle\alpha_0|\alpha_1\rangle|^2}.
$$

Therefore

$$
\boxed{
P_s\leq\frac12\left(1+
\sqrt{1-|\langle\alpha_0|\alpha_1\rangle|^2}\right)},
$$

and the positive/negative eigenspace measurement attains equality.

The right side equals one exactly when $|\langle\alpha_0|\alpha_1\rangle|=0$. Thus two pure states are perfectly distinguishable exactly when they are orthogonal.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [15C](../../15c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [Hamiltonian](../../../../../../hamiltonian.md) [functional](../../../../../../functional.md) is

$$
H[\psi,\psi^*]=\int\left[\frac{\hbar^2}{2m}|\nabla\psi|^2+V_{\rm ext}|\psi|^2+\frac U2|\psi|^4\right]d^3x.
$$

Treating the field and its [complex conjugate](../../../../../../complex-conjugate.md) as independent variables, and integrating the [gradient](../../../../../../gradient.md) term by parts with periodic, decaying or fixed-field boundary conditions, gives

$$
\frac{\delta H}{\delta\psi^*}=-\frac{\hbar^2}{2m}\nabla^2\psi+V_{\rm ext}\psi+U|\psi|^2\psi.
$$

Thus $i\hbar\psi_t=\delta H/\delta\psi^*$ is the [Gross–Pitaevskii equation](../../../../../../gross-pitaevskii-equation.md). The factor $1/2$ in the interaction energy avoids counting each pair twice.

At prescribed particle number, minimize $H$ subject to $N=\int|\psi|^2d^3x$. Introducing the [chemical potential](../../../../../../chemical-potential.md) as a [Lagrange multiplier](../../../../../../lagrange-multiplier.md), the variation of $H-\mu N$ vanishes at a ground-state profile $\psi_0$, proving

$$
\boxed{\left[-\frac{\hbar^2}{2m}\nabla^2+V_{\rm ext}+U|\psi_0|^2\right]\psi_0=\mu\psi_0.}
$$

The corresponding time-dependent field is $\psi(\mathbf x,t)=e^{-i\mu t/\hbar}\psi_0(\mathbf x)$. A solution of this stationary equation is only a candidate [ground state](../../../../../../ground-state.md); the [ground state](../../../../../../ground-state.md) is the minimizer among all fields satisfying the normalization. For the uniform repulsive gas in a periodic volume, the [gradient](../../../../../../gradient.md) energy is nonnegative and $\int n^2d^3x\ge N^2/\mathcal V$, so the constant-density, constant-phase state is indeed the minimum. The uniform-background solutions below assume $U>0$ and a positive background density.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 83](../../../paper-83-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

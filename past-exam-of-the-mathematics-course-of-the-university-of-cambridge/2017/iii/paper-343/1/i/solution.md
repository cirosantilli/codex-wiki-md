<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The $-\mu\psi$ term means that the generator is the [grand potential](../../../../../../grand-potential.md), rather than just the physical [energy](../../../../../../energy.md). With boundary variations vanishing, the [Hamiltonian](../../../../../../hamiltonian.md) [functional](../../../../../../functional.md) is

$$
\boxed{H[\psi,\psi^*]=\int\left[\frac{\hbar^2}{2m}|\nabla\psi|^2+\frac g2|\psi|^4-\mu|\psi|^2\right]d^d x.}
$$

Its [functional derivative](../../../../../../functional-derivative.md) is

$$
\frac{\delta H}{\delta\psi^*}=-\frac{\hbar^2}{2m}\nabla^2\psi+(g|\psi|^2-\mu)\psi,
$$

so the [Gross–Pitaevskii equation](../../../../../../gross-pitaevskii-equation.md) is $i\hbar\psi_t=\delta H/\delta\psi^*$. Treating $\psi$ and $\psi^*$ as independent variables in this variation gives the factor $g$, not $2g$.

For repulsive interactions $g>0$ and $\mu>0$, complete the square in the local [energy](../../../../../../energy.md):

$$
\frac g2 n^2-\mu n=\frac g2\left(n-\frac\mu g\right)^2-\frac{\mu^2}{2g}.
$$

The [gradient](../../../../../../gradient.md) contribution is nonnegative, so the homogeneous [ground state](../../../../../../ground-state.md) has arbitrary constant [complex argument](../../../../../../argument-complex-analysis.md) and

$$
\boxed{n_0=\frac\mu g,\qquad \psi_0=\sqrt{n_0}e^{i\theta_0}.}
$$

The infinite-volume constant may be subtracted to define a relative [grand potential](../../../../../../grand-potential.md); it does not affect the [functional derivative](../../../../../../functional-derivative.md). At fixed particle number one instead minimizes the physical [energy](../../../../../../energy.md) $H+\mu N$, with $\mu$ as its [Lagrange multiplier](../../../../../../lagrange-multiplier.md). For $g>0$, $\mu\leq0$ the grand-potential minimum over $n\geq0$ is the vacuum $n=0$. For $g<0$ the displayed unconstrained [functional](../../../../../../functional.md) is unbounded below; the positive-density stable uniform state assumed in the following parts requires repulsion.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 343](../../../paper-343-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

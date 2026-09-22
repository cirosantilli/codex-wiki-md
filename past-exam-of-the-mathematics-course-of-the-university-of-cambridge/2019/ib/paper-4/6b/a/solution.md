<h1 id="6b/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a [wavefunction](../../../../../../wave-function.md) $\Psi(x,t)$, the [probability density](../../../../../../probability-density.md) and [probability current](../../../../../../probability-current.md) are

$$
\rho=|\Psi|^2,
\qquad
j=\frac{\hbar}{2mi}\left(\Psi^*\frac{\partial\Psi}{\partial x}-\Psi\frac{\partial\Psi^*}{\partial x}\right).
$$

Multiply the [Schrödinger equation](../../../../../../schrodinger-equation.md) by $\Psi^*$, multiply its [complex conjugate](../../../../../../complex-conjugate.md) by $\Psi$, and subtract. The real [potential energy](../../../../../../potential-energy.md) terms cancel, leaving

$$
\frac{\partial|\Psi|^2}{\partial t}
=-\frac{\partial}{\partial x}
\left[\frac{\hbar}{2mi}
\left(\Psi^*\Psi_x-\Psi\Psi_x^*\right)\right],
$$

which is the [probability continuity equation](../../../../../../probability-continuity-equation.md) $\rho_t+j_x=0$.

For a [stationary state](../../../../../../stationary-state.md), $\rho_t=0$, so $j_x=0$ and $j$ is constant in space. A [normalizable wavefunction](../../../../../../normalizable-wavefunction.md) has vanishing current at spatial infinity, forcing this constant to be zero. By contrast the nonnormalizable [plane wave](../../../../../../plane-wave.md)

$$
\Psi(x,t)=A e^{i(kx-\omega t)}
$$

has stationary density $|A|^2$ and nonzero current

$$
\boxed{j=\frac{\hbar k}{m}|A|^2}
$$

when $k\ne0$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6B](../../6b.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

<h1 id="6b/solution">Solution</h1>

↑ **Parent:** [6B](../6b.md)

For the [wavefunction](../../../../../wave-function.md) of a particle of [mass](../../../../../mass.md) $m$, the [probability density](../../../../../probability-density.md) and [probability current](../../../../../probability-current.md) are

$$
\boxed{\rho=\Psi^*\Psi,\qquad j=\frac{\hbar}{2mi}(\Psi^*\Psi_x-\Psi\Psi_x^*)=\frac\hbar m\operatorname{Im}(\Psi^*\Psi_x).}
$$

For a real potential $V$, the [Time-dependent Schrödinger equation](../../../../../time-dependent-schrodinger-equation.md) and its [complex conjugate](../../../../../complex-conjugate.md) read

$$
i\hbar\Psi_t=-\frac{\hbar^2}{2m}\Psi_{xx}+V\Psi,\qquad -i\hbar\Psi_t^*=-\frac{\hbar^2}{2m}\Psi_{xx}^*+V\Psi^*.
$$

Multiplying by $\Psi^*$ and $\Psi$ respectively yields

$$
\rho_t=\frac{i\hbar}{2m}(\Psi^*\Psi_{xx}-\Psi\Psi_{xx}^*)=-j_x.
$$

The potential terms cancel because $V$ is real. This is the [continuity equation](../../../../../continuity-equation.md), expressing local conservation of probability.

For the given [superposition](../../../../../superposition-principle.md) the common time phase cancels in $\Psi^*\Psi_x$, and

$$
\Psi^*\Psi_x=ik(1-|R|^2)+ik(R^*e^{2ikx}-Re^{-2ikx}).
$$

The expression in the second parentheses is purely imaginary, so the second term is real and contributes nothing to the [probability current](../../../../../probability-current.md). Thus

$$
\boxed{j=\frac{\hbar k}{m}(1-|R|^2).}
$$

It is the incoming [probability current](../../../../../probability-current.md) minus the reflected [probability current](../../../../../probability-current.md).

## ↑ Ancestors (10)

1. [6B](../6b.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

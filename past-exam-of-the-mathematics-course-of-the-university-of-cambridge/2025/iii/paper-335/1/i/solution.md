<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [phase screen](../../../../../../phase-screen.md) adds the phase accumulated across its thickness, so the reduced field just after the screen is

$$
E(0,z)=e^{ik\xi w(z)}.
$$

For a zero-mean random variable $w$ with a [normal distribution](../../../../../../normal-distribution.md) and variance $\sigma^2$, its [characteristic function](../../../../../../characteristic-function.md) gives

$$
\boxed{\langle E(0,z)\rangle
=\exp\left(-\frac12k^2\xi^2\sigma^2\right).}
$$

The same expression is approximately valid for a non-Gaussian weak fluctuation: the [cumulant expansion](../../../../../../cumulant-expansion.md) begins with $-k^2\xi^2\sigma^2/2$, while higher cumulants give higher-order corrections.

For $x>0$, every realization obeys the [parabolic wave equation](../../../../../../parabolic-wave-equation.md)

$$
2ikE_x+E_{zz}=0.
$$

Linearity permits ensemble averaging, so

$$
\boxed{2ik\partial_x\langle E\rangle
+\partial_z^2\langle E\rangle=0.}
$$

The initial mean is independent of $z$, hence diffraction does not change it and $\langle E(x,z)\rangle=\exp(-k^2\xi^2\sigma^2/2)$ for every $x\geq0$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 335](../../../paper-335-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

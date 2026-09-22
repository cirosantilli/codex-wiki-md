<h1 id="6b/solution">Solution</h1>

↑ **Parent:** [6B](../6b.md)

Put $D=1+i\hbar t/m$ and write the [Gaussian wave packet](../../../../../gaussian-wave-packet.md) as $\psi=\pi^{-1/4}D^{-1/2}e^{-x^2/(2D)}$. Differentiation gives

$$
\frac{\psi_t}{\psi}=\frac{i\hbar}{m}\left(-\frac1{2D}+\frac{x^2}{2D^2}\right),\qquad
\frac{\psi_{xx}}{\psi}=\frac{x^2}{D^2}-\frac1D.
$$

Hence $\boxed{i\hbar\psi_t=-(\hbar^2/2m)\psi_{xx}}$, the free [Time-dependent Schrödinger equation](../../../../../time-dependent-schrodinger-equation.md).

With $\tau=\hbar t/m$, its [probability density](../../../../../probability-density.md) is

$$
|\psi|^2=\frac{1}{\sqrt{\pi(1+\tau^2)}}\exp\left(-\frac{x^2}{1+\tau^2}\right).
$$

The stated [Gaussian integral](../../../../../gaussian-integral.md) shows its integral is one. Symmetry gives $\langle x\rangle=0$; differentiating that Gaussian integral with respect to its coefficient gives $\langle x^2\rangle=(1+\tau^2)/2$. Thus the position [standard deviation](../../../../../standard-deviation.md) is

$$
\boxed{\Delta x=\sqrt{\frac{1+(\hbar t/m)^2}{2}}.}
$$

**It is not a stationary state:** its probability density changes with time as the packet spreads. A [stationary state](../../../../../stationary-state.md) would have only an overall time-dependent phase and a fixed position density.

## ↑ Ancestors (10)

1. [6B](../6b.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

<h1 id="4c/solution">Solution</h1>

↑ **Parent:** [4C](../4c.md)

The one-dimensional [Time-dependent Schrödinger equation](../../../../../time-dependent-schrodinger-equation.md) for a [wavefunction](../../../../../wave-function.md) in a real potential is

$$
i\hbar\frac{\partial\Psi}{\partial t}
=-\frac{\hbar^2}{2m}\frac{\partial^2\Psi}{\partial x^2}+U\Psi.
$$

Multiplying this equation by $\Psi^*$, multiplying its [complex conjugate](../../../../../complex-conjugate.md) by $\Psi$, and subtracting gives the [probability continuity equation](../../../../../probability-continuity-equation.md)

$$
\frac{\partial |\Psi|^2}{\partial t}+\frac{\partial j}{\partial x}=0,
\qquad
j=\frac{\hbar}{2mi}\left(\Psi^*\frac{\partial\Psi}{\partial x}
-\Psi\frac{\partial\Psi^*}{\partial x}\right).
$$

If $\Psi$ and its first [derivative](../../../../../derivative.md) decay sufficiently rapidly as $x\to\pm\infty$, then the [probability current](../../../../../probability-current.md) $j$ vanishes at both ends. Integrating the continuity equation and using the [fundamental theorem of calculus](../../../../../fundamental-theorem-of-calculus.md) yields

$$
\frac d{dt}\int_{-\infty}^{\infty}|\Psi(x,t)|^2\,dx
=-j(\infty,t)+j(-\infty,t)=0.
$$

This [conservation of quantum probability](../../../../../conservation-of-quantum-probability.md) is required by the [Born rule](../../../../../born-rule.md): once a [normalizable wavefunction](../../../../../normalizable-wavefunction.md) has total probability one, its time evolution must preserve that normalization.

For the stated [Gaussian wave packet](../../../../../gaussian-wave-packet.md), put $\beta=\hbar t/m$. Since

$$
f(t)=\frac1{\alpha+i\beta},
\qquad
|f(t)|=\frac1{\sqrt{\alpha^2+\beta^2}},
\qquad
\operatorname{Re}f(t)=\frac{\alpha}{\alpha^2+\beta^2},
$$

its squared [modulus](../../../../../modulus.md) is

$$
|\Psi(x,t)|^2
=\frac{C^2}{\sqrt{\alpha^2+\beta^2}}
\exp\left(-\frac{\alpha x^2}{\alpha^2+\beta^2}\right).
$$

The [Gaussian integral](../../../../../gaussian-integral.md) then gives

$$
\int_{-\infty}^{\infty}|\Psi(x,t)|^2\,dx
=\frac{C^2}{\sqrt{\alpha^2+\beta^2}}
\sqrt{\frac{\pi(\alpha^2+\beta^2)}{\alpha}}
=\boxed{C^2\sqrt{\frac\pi\alpha}},
$$

which is independent of time, as required.

## ↑ Ancestors (10)

1. [4C](../4c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

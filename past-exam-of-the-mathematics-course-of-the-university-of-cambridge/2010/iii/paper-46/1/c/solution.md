<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Apply the [Poisson summation formula](../../../../../../poisson-summation-formula.md) in the convention supplied, taking

$$
f(x)=\exp\left(-\frac{2\pi^2i\hbar T}{\Lambda}x^2\right),\qquad\Theta=\Delta.
$$

Completing the square in its [Fourier transform](../../../../../../fourier-transform.md) and evaluating the analytically continued [Gaussian integral](../../../../../../gaussian-integral.md) gives

$$
\widetilde f(k)=\sqrt{\frac{\Lambda}{2\pi i\hbar T}}\exp\left(\frac{i\Lambda k^2}{2\hbar T}\right).
$$

Thus the spectral sum becomes

$$
\boxed{K(\theta_f,\theta_i;T)=\sqrt{\frac{\Lambda}{2\pi i\hbar T}}\sum_{m\in\mathbb Z}e^{iS_m/\hbar}.}
$$

The square-root branch is fixed by continuation from positive imaginary-time damping. Each term is the classical contribution of part (b), multiplied by the same fluctuation prefactor. Since the [action](../../../../../../action.md) is quadratic, writing $\theta=\theta_m+\eta$ with $\eta(0)=\eta(T)=0$ removes the cross term and leaves a free Gaussian fluctuation integral independent of $m$. This [real-time winding representation of a quantum rotor kernel](../../../../../../real-time-winding-representation-of-a-quantum-rotor-kernel.md) is exact, rather than only a leading semiclassical approximation.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 46](../../../paper-46-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

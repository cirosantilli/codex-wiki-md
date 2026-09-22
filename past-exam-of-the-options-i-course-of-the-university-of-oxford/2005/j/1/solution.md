<h1 id="j/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [time-independent Schrödinger equation](../../../../time-independent-schrodinger-equation.md) is

$$
-\frac{\hbar^2}{2m}\psi''(x)+\frac12m\omega^2x^2\psi(x)=E\psi(x).
$$

Put $\alpha=m\omega/\hbar$. For $\psi=e^{-\alpha x^2/2}$, differentiation gives $\psi''=(\alpha^2x^2-\alpha)\psi$. Substitution cancels the terms in $x^2$ and leaves $E_0=\hbar^2\alpha/(2m)=\hbar\omega/2$.

The [Gaussian integral](../../../../gaussian-integral.md) gives $\int e^{-\alpha x^2}\,dx=\sqrt{\pi/\alpha}$. Hence a normalized [wave function](../../../../wave-function-split.md) is

$$
\boxed{\psi_0(x)=\left(\frac{m\omega}{\pi\hbar}\right)^{1/4}\exp\left(-\frac{m\omega x^2}{2\hbar}\right).}
$$

Multiplication by any constant of modulus one gives the same [quantum state](../../../../quantum-state.md). The [position](../../../../position.md) [probability density](../../../../probability-density.md) is $|\psi_0|^2=\sqrt{\alpha/\pi}e^{-\alpha x^2}$. Its first [moment](../../../../moment.md) vanishes by oddness. [Integration by parts](../../../../integration-by-parts.md) gives $\int x^2e^{-\alpha x^2}\,dx=(2\alpha)^{-1}\int e^{-\alpha x^2}\,dx$, with the boundary term zero. Therefore

$$
\boxed{\langle x\rangle=0,\qquad\operatorname{Var}(x)=\langle x^2\rangle=\frac{\hbar}{2m\omega}.}
$$

## ↑ Ancestors (12)

1. [1](../1.md)
2. [J](../../j.md)
3. [2005](../../../2005-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

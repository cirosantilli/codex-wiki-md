<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Fourier transform of a derivative](../../../../../fourier-transform-of-a-derivative.md) is $i\omega$ times the transform under the stated convention. Transforming the [linear ordinary differential equation](../../../../../linear-ordinary-differential-equation-split.md) gives

$$
(-\omega^2+5i\omega+6)\widetilde x=\widetilde F,
\qquad\boxed{R(\omega)=\frac1{(i\omega+2)(i\omega+3)}.}
$$

The applied [force](../../../../../force-split.md) is $F(t)=H(t)e^{-t}$, with $H$ the [Heaviside step function](../../../../../heaviside-step-function.md), so $\widetilde F=(1+i\omega)^{-1}$. Partial fractions give

$$
\widetilde x=\frac{1/2}{1+i\omega}-\frac1{2+i\omega}+\frac{1/2}{3+i\omega}.
$$

Using the transform pair $H(t)e^{-ct}\leftrightarrow(c+i\omega)^{-1}$ yields

$$
\boxed{x(t)=H(t)\left(\tfrac12e^{-t}-e^{-2t}+\tfrac12e^{-3t}\right).}
$$

Its value and first [derivative](../../../../../derivative.md) both vanish at $t=0^+$, so the joining introduces no spurious [Dirac delta](../../../../../dirac-delta-function.md) terms. Equivalently, this is the [convolution](../../../../../convolution.md) of the [force](../../../../../force-split.md) with the causal [impulse response](../../../../../impulse-response.md) $H(t)(e^{-2t}-e^{-3t})$.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

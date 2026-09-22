<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $T=t-t'$. [momentum](../../../../../momentum-split.md) [eigenstates](../../../../../eigenstate.md) evolve with [energy](../../../../../energy-split.md) $p^2/(2m)$, so the retarded [momentum](../../../../../momentum-split.md) kernel is $\theta(T)\delta(p-p')e^{-ip^2T/(2m\hbar)}$. Its [Fourier transform](../../../../../fourier-transform-split.md) reduces to

$$
K_0=\frac{\theta(T)}{2\pi\hbar}\int dp\,
\exp\left[\frac i\hbar\left(p(x-x')-\frac{p^2T}{2m}\right)\right].
$$

Completing the square and defining the oscillatory [Gaussian integral](../../../../../gaussian-integral.md) by a convergent limiting prescription gives

$$
\boxed{K_0=\theta(T)\sqrt{\frac{m}{2\pi i\hbar T}}
\exp\left[\frac{im(x-x')^2}{2\hbar T}\right]}.
$$

For $T>0$ the [square root](../../../../../square-root.md) has [quantum phase](../../../../../quantum-phase.md) $e^{-i\pi/4}$. As $T\downarrow0$, this kernel tends to $\delta(x-x')$ in the distributional sense. Differentiating the [Heaviside step function](../../../../../heaviside-step-function.md) consequently supplies the required $i\hbar\delta(T)\delta(x-x')$ source; an extra $-i/\hbar$ factor would correspond to a different Green-function convention.

## ↑ Ancestors (15)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2013](../../../split.md)
5. [Past exam of the theoretical physics II course of the University of Cambridge](../../../../split.md)
6. [Theoretical Physics II course of the University of Cambridge](../../../../../theoretical-physics-ii-course-of-the-university-of-cambridge.md)
7. [Theoretical Physics course of the University of Cambridge](../../../../../theoretical-physics-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../split.md)

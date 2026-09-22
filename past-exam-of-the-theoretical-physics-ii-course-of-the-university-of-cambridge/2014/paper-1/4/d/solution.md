<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write $T_p=p^2/(2m)$ and $V=m\omega^2x^2/2$. Dropping [commutators](../../../../../commutator.md) of order $\beta^2$ permits $e^{-\beta H}\simeq e^{-\beta V}e^{-\beta T_p}$. With $\langle x|p\rangle=e^{ipx/\hbar}/\sqrt{2\pi\hbar}$, the [momentum](../../../../../momentum-split.md) Gaussian gives

$$
\langle x|e^{-\beta H}|x'\rangle\simeq
\sqrt{\frac{m}{2\pi\beta\hbar^2}}\exp\left[-\frac{m(x-x')^2}{2\beta\hbar^2}-\frac{\beta m\omega^2x^2}{2}\right].
$$

Integrating the diagonal yields $Z\simeq1/(\beta\hbar\omega)$, so the [leading high-temperature density kernel](../../../../../leading-high-temperature-density-kernel.md) is

$$
\boxed{\langle x|\rho|x'\rangle\simeq
\omega\sqrt{\frac{\beta m}{2\pi}}\exp\left[-\frac{m(x-x')^2}{2\beta\hbar^2}-\frac{\beta m\omega^2x^2}{2}\right]}.
$$

This unsymmetrized product has an apparent off-diagonal asymmetry at the omitted order; reversing the product puts $x'$ in the potential factor. A manifestly [Hermitian](../../../../../hermitian-operator.md) approximation uses $e^{-\beta V/2}e^{-\beta T_p}e^{-\beta V/2}$, replacing $\beta m\omega^2x^2/2$ by $\beta m\omega^2(x^2+x'^2)/4$ with the same leading normalization. The condition is $\beta\hbar\omega\ll1$; the Gaussian off-diagonal width is of order $\hbar\sqrt{\beta/m}$.

## ↑ Ancestors (15)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2014](../../../split.md)
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

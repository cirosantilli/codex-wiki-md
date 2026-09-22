<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $F(\omega)=\widetilde f(\omega)$ to distinguish the [Fourier transform](../../../../../fourier-transform-split.md) from the original function. [Integration by parts](../../../../../integration-by-parts.md), using the stated decay, gives

$$
\widehat{f'}(\omega)=\big[f(t)e^{-i\omega t}\big]_{-\infty}^{\infty}+i\omega\int_{-\infty}^{\infty}f(t)e^{-i\omega t}\,dt=i\omega F(\omega).
$$

Applying the same argument to $f'$ gives $\widehat{f''}=i\omega\widehat{f'}=-\omega^2F$. Differentiation with respect to the frequency gives

$$
F'(\omega)=\int_{-\infty}^{\infty}(-it)f(t)e^{-i\omega t}\,dt=-i\widehat{tf}(\omega).
$$

Consequently

$$
\boxed{\widehat{f'}=i\omega F,\qquad\widehat{f''}=-\omega^2F,\qquad\widehat{tf}=iF'.}
$$

The classical steps require existence of the relevant integrals and justification for differentiation under the integral, for example sufficient integrability of $f$, its derivatives and $tf$. The same identities extend to [tempered distributions](../../../../../tempered-distribution.md), which is the useful interpretation in part (c).

## ↑ Ancestors (13)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

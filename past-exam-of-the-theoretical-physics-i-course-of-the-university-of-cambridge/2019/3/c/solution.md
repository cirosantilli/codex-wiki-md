<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Choose the real representative $v=\psi_0=\sqrt{\mu/g}$. For $\psi=v+\chi$,

$$
|\psi|^2=v^2+v(\chi+\chi^*)+|\chi|^2,
$$

and the fourth power through quadratic order is

$$
|\psi|^4=v^4+2v^3(\chi+\chi^*)+2v^2|\chi|^2+v^2(\chi+\chi^*)^2+O(\chi^3).
$$

In $\mu|\psi|^2-g|\psi|^4/2$, the linear terms and the $|\chi|^2$ terms cancel because $gv^2=\mu$. The remaining potential contribution is $\mu^2/(2g)-\mu(\chi+\chi^*)^2/2$.

The time-derivative contribution is

$$
\frac{i\hbar}{2}(\psi^*\dot\psi-\psi\dot\psi^*)
=\frac{i\hbar v}{2}\partial_t(\chi-\chi^*)+\frac{i\hbar}{2}(\chi^*\dot\chi-\chi\dot\chi^*).
$$

Its first term is a [total derivative](../../../../total-derivative.md) and contributes only a temporal [boundary term](../../../../boundary-term.md) for fixed endpoint fields. Since $v$ is uniform, the gradient contribution is simply $-\hbar^2|\nabla\chi|^2/(2M)$. Dropping that boundary term and the constant, the [quadratic condensate fluctuation Lagrangian](../../../../quadratic-condensate-fluctuation-lagrangian.md) is

$$
\boxed{\mathcal L_2=\frac{i\hbar}{2}(\chi^*\dot\chi-\chi\dot\chi^*)-\frac{\hbar^2}{2M}\nabla\chi^*\cdot\nabla\chi-\frac\mu2(\chi+\chi^*)^2.}
$$

The omitted cubic and quartic interactions describe scattering between these small fluctuations; they do not enter the linear [normal mode](../../../../normal-mode.md) calculation.

## ↑ Ancestors (14)

1. [C](../c.md)
2. [3](../../3.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the theoretical physics I course of the University of Cambridge](../../../split.md)
5. [Theoretical Physics I course of the University of Cambridge](../../../../theoretical-physics-i-course-of-the-university-of-cambridge.md)
6. [Theoretical Physics course of the University of Cambridge](../../../../theoretical-physics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../list-of-universities.md)
14. [Codex Wiki](../../../../split.md)

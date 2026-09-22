<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

With the PDF's inverse [Fourier transform](../../../../fourier-transform-split.md) convention, the derivatives act as

$$
\partial_t\mapsto-i\omega,\qquad\partial_x\mapsto-ik,
$$

so its forced differential operator becomes $\omega^2-k^2+i\gamma\omega k^2$. Thus

$$
\boxed{\widehat G(k,\omega)=\frac1{\omega^2-k^2+i\gamma k^2\omega}.}
$$

For the physical impulse response choose the [retarded fundamental solution](../../../../retarded-fundamental-solution.md), vanishing before $t=0$. For $k\ne0$ and $\gamma>0$, its poles lie in the lower half-plane. The [retarded Fourier pole prescription](../../../../retarded-fourier-pole-prescription.md) $\omega\mapsto\omega+i0$ specifies the zero mode and the zero-damping limit as well; a Green function without a temporal or boundary prescription would otherwise permit homogeneous additions.

This is the [Kelvin-Voigt rod Green function](../../../../kelvin-voigt-rod-green-function.md). Multiplying the homogeneous real-space equation by $-1$ gives

$$
\phi_{tt}-\phi_{xx}-\gamma\phi_{txx}=0.
$$

A spatial [Fourier mode](../../../../fourier-mode.md) therefore satisfies $\ddot\phi_k+\gamma k^2\dot\phi_k+k^2\phi_k=0$: positive $\gamma$ really damps the motion. For sufficiently decaying fields its [energy](../../../../energy-split.md) satisfies

$$
\frac d{dt}\frac12\int(\phi_t^2+\phi_x^2)\,dx=-\gamma\int\phi_{tx}^2\,dx\leq0.
$$

This checks the sign of the imaginary term in $\widehat G$ independently of the transform calculation.

## ↑ Ancestors (14)

1. [C](../c.md)
2. [4](../../4.md)
3. [2018](../../../2018-split.md)
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

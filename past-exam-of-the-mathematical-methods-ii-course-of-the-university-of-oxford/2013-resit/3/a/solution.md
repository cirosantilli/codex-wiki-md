<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For one sine mode, $y_{xx}=-k_n^2A_n\sin(k_nx)\cos(\omega_nt)$ and $y_{tt}=-\omega_n^2A_n\sin(k_nx)\cos(\omega_nt)$. The [wave equation on a string](../../../../wave-equation-on-a-string.md) therefore holds when

$$
\boxed{\omega_n^2=\frac T\mu k_n^2,\qquad \omega_n=vk_n,\quad v=\sqrt{T/\mu}.}
$$

The [superposition principle](../../../../superposition-principle.md) gives the same equation for the sum, assuming enough regularity to differentiate termwise, or interpreting finite-energy data in the usual modal sense. Fixed endpoints require $\sin(k_nL)=0$, so $k_n=n\pi/L$. Every cosine time factor has zero time derivative at $t=0$, giving the held-at-rest initial condition.

The coefficients must represent the actual held profile $f(x)$ through its [Fourier sine series](../../../../fourier-sine-series.md), $A_n=(2/L)\int_0^Lf(x)\sin(n\pi x/L)dx$ for $n\geq1$. Thus the series accommodates the displacement initial condition once these coefficients are chosen; it does not select an unspecified initial shape by itself. The printed $n=0$ term is identically zero because $\sin0=0$, so the nontrivial fixed-end modes start at $n=1$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2013 resit](../../../2013-resit-split.md)
4. [Past exam of the mathematical methods II course of the University of Oxford](../../../split.md)
5. [Mathematical methods II course of the University of Oxford](../../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

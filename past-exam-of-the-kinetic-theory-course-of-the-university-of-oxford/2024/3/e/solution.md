<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Represent the perturber by the periodic [Dirac delta function](../../../../dirac-delta-function.md) at $\mathbf x_p+\mathbf v_pt$. With spatial [Fourier series](../../../../fourier-series-split.md) coefficient normalized by $L^{-3}$, its nonzero density coefficients are

$$
\rho_{p,\mathbf k}(t)=\frac{m_p}{L^3}e^{-i\mathbf k\cdot\mathbf x_p}e^{-i\mathbf k\cdot\mathbf v_pt},\qquad t\geq0.
$$

The mean density is subtracted as in [d](../d.md). The [Poisson equation for Newtonian gravity](../../../../poisson-equation-for-newtonian-gravity.md) gives

$$
\delta\Phi_{\mathbf k}^{\mathrm{ext}}(t)=C_{\mathbf k}e^{-iat},\qquad C_{\mathbf k}=-\frac{4\pi Gm_p}{L^3k^2}e^{-i\mathbf k\cdot\mathbf x_p},\qquad a=\mathbf k\cdot\mathbf v_p.
$$

The perturbation is zero before switch-on. For $\operatorname{Im}\omega>0$, its [Laplace transform](../../../../laplace-transform.md) is

$$
\int_0^\infty e^{i(\omega-a)t}\,dt=-\frac1{i(\omega-a)}=\frac1{i(a-\omega)}.
$$

Hence

$$
\boxed{\widetilde{\delta\Phi}_{\mathbf k}^{\mathrm{ext}}(\omega)=-\frac{4\pi Gm_p}{L^3k^2}e^{-i\mathbf k\cdot\mathbf x_p}\frac1{i(\mathbf k\cdot\mathbf v_p-\omega)}.}
$$

The switch-on creates a forcing pole at the real [frequency](../../../../frequency.md) $a$, approached causally from the original upper inversion contour.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [3](../../3.md)
3. [2024](../../../2024-split.md)
4. [Past exam of the kinetic theory course of the University of Oxford](../../../split.md)
5. [Kinetic theory course of the University of Oxford](../../../../kinetic-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

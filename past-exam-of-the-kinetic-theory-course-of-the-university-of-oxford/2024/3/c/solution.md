<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the stated [Fourier series](../../../../fourier-series-split.md) normalization, so $g(\boldsymbol\theta,\mathbf J,t)=\sum_{\mathbf n}g_{\mathbf n}(\mathbf J,t)e^{i\mathbf n\cdot\boldsymbol\theta}$. Then [b](../b.md) gives

$$
\partial_t\delta f_{\mathbf n}+i\mathbf n\cdot\boldsymbol\Omega\,\delta f_{\mathbf n}-i\mathbf n\cdot\frac{\partial f_0}{\partial\mathbf J}\,\delta\Phi_{\mathbf n}^{\mathrm{tot}}=0.
$$

For the [Laplace transform](../../../../laplace-transform.md) with kernel $e^{i\omega t}$, [integration by parts](../../../../integration-by-parts.md) yields

$$
\int_0^\infty e^{i\omega t}\partial_t\delta f_{\mathbf n}\,dt=-\delta f_{\mathbf n}(0)-i\omega\widetilde{\delta f}_{\mathbf n}.
$$

The upper boundary vanishes for sufficiently large $\operatorname{Im}\omega>0$, and the initial term is zero by hypothesis. Thus

$$
i(\mathbf n\cdot\boldsymbol\Omega-\omega)\widetilde{\delta f}_{\mathbf n}=i\mathbf n\cdot\frac{\partial f_0}{\partial\mathbf J}\,\widetilde{\delta\Phi}_{\mathbf n}^{\mathrm{tot}},
$$

or

$$
\boxed{\widetilde{\delta f}_{\mathbf n}(\mathbf J,\omega)=-\mathbf n\cdot\frac{\partial f_0}{\partial\mathbf J}\frac{\widetilde{\delta\Phi}_{\mathbf n}^{\mathrm{tot}}(\mathbf J,\omega)}{\omega-\mathbf n\cdot\boldsymbol\Omega(\mathbf J)},\qquad \boldsymbol\Omega=\frac{\partial H_0}{\partial\mathbf J}.}
$$

The denominator identifies the [orbital resonance](../../../../orbital-resonance.md) between the perturbation and unperturbed orbital [frequencies](../../../../frequency.md). The zero harmonic has no driving term and remains zero with these initial data.

## ↑ Ancestors (12)

1. [C](../c.md)
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

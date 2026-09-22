# Cooling of an initially uniform square

↑ **Parent:** [Heat equation](heat-equation.md)

For a square of side $\ell$ initially at constant temperature $T_0$, held at zero boundary temperature for $t>0$, the [heat equation](heat-equation.md) $T_t=\kappa\Delta T$ with $\kappa>0$ has solution

$$
T=\frac{16T_0}{\pi^2}\sum_{\substack{m,n\geq1\\m,n\text{ odd}}}\frac{\sin(m\pi x/\ell)\sin(n\pi y/\ell)}{mn}\,e^{-\kappa\pi^2(m^2+n^2)t/\ell^2}.
$$

The [double Fourier sine series](double-fourier-sine-series.md) of the initial constant gives the coefficients. The spatial modes are [Dirichlet Laplacian eigenfunctions](dirichlet-laplacian-eigenfunction.md), so [separation of variables](separation-of-variables.md) gives their decay rates. At late times the $(1,1)$ mode dominates, giving the displayed profile; the next nonzero decay exponent is $10\kappa\pi^2/\ell^2$. At early times the series approaches the constant at each interior point and in [L2 space](l2-space-is-a-hilbert-space.md), while the boundary remains at zero. An instantaneous change to the boundary condition therefore need not produce a solution continuous at the initial boundary in space-time.

## ↑ Ancestors (7)

1. [Heat equation](heat-equation.md)
2. [Diffusion equation](diffusion-equation-split.md)
3. [Partial differential equation](partial-differential-equation-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2008/paper-1/2/c/solution.md)

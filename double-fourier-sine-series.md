# Double Fourier sine series

↑ **Parent:** [Fourier sine series](fourier-sine-series.md)

On a rectangle $(0,L_x)\times(0,L_y)$, products of the one-dimensional [Fourier sine basis](fourier-sine-basis.md) give an orthogonal basis of [L2 space](l2-space-is-a-hilbert-space.md). [Fourier orthogonality](fourier-orthogonality.md) in each variable gives

$$
c_{mn}=\frac4{L_xL_y}\int_0^{L_x}\int_0^{L_y}f(x,y)\sin\frac{m\pi x}{L_x}\sin\frac{n\pi y}{L_y}\,dy\,dx.
$$

For a constant function one, these coefficients are $4[1-(-1)^m][1-(-1)^n]/(\pi^2mn)$: only odd indices occur. The product modes vanish on the rectangle's boundary, making them natural [Dirichlet Laplacian eigenfunctions](dirichlet-laplacian-eigenfunction.md). In the [heat equation](heat-equation.md), their amplitudes decay as $e^{-\kappa\pi^2(m^2/L_x^2+n^2/L_y^2)t}$. Initial data not vanishing at the boundary are still represented in the interior and in the square-integrable sense; the positive-time boundary values need not agree continuously with the initially assigned boundary values.

## ↑ Ancestors (6)

1. [Fourier sine series](fourier-sine-series.md)
2. [Fourier series](fourier-series-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Cooling of an initially uniform square](cooling-of-an-initially-uniform-square.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2008/paper-1/2/b/solution.md)

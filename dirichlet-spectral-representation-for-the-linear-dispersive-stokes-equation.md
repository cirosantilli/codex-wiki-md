# Dirichlet spectral representation for the linear dispersive Stokes equation

↑ **Parent:** [Half-line linear dispersive Stokes global relation](half-line-linear-dispersive-stokes-global-relation.md)

Let $A_j$ be the weights of the [cubic Stokes dispersion symmetry](cubic-stokes-dispersion-symmetry.md) and set $F(k)=\sum_jA_j(k)\widehat q_0(\nu_j(k))$. Orient $\partial D_+$ with $D_+$ on its left. Evaluating the [global relation](global-relation-for-a-linear-boundary-value-problem.md) at its two lower-half-plane roots and interpolating the linear expression $ikG_1+G_2$ removes both unknown boundary traces. The resulting [Fokas method](fokas-method.md) formula is

$$
q(x,t)=\frac1{2\pi}\int_{\mathbb R}e^{ikx-\omega t}\widehat q_0(k)\,dk+\frac1{2\pi}\int_{\partial D_+}e^{ikx-\omega t}\bigl[(1-3k^2)G_0(k,t)-F(k)\bigr]dk.
$$

The discarded transform of the solution is [holomorphic](complex-differentiability-at-a-point.md) in $D_+$ and has zero [integral](integral.md) after closing its [contour](complex-integration-contour.md) for $x>0$. Initial compatibility and sufficient smoothness and spatial decay are required. At the boundary, use a fixed time horizon later than $t$ before [Fourier inversion](fourier-inversion-theorem.md), to avoid an endpoint half-value.

## ↑ Ancestors (9)

1. [Half-line linear dispersive Stokes global relation](half-line-linear-dispersive-stokes-global-relation.md)
2. [Global relation for a linear boundary value problem](global-relation-for-a-linear-boundary-value-problem.md)
3. [Boundary value problem](boundary-value-problem.md)
4. [Ordinary differential equation](ordinary-differential-equation.md)
5. [Differential equation](differential-equation-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-71/1/c/solution.md)

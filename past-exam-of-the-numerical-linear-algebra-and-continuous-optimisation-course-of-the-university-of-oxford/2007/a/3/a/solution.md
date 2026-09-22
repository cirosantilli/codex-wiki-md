<h1 id="a/3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [multigrid method](../../../../../multigrid-method-split.md) alternates local error damping with correction on coarser grids. For clarity write $A_h=h^{-2}$ times the five-point stencil and $A_hu_h=f_h$, incorporating Dirichlet boundary data into the right side. One two-grid cycle proceeds as follows.

- Apply a few smoothing sweeps, for example [weighted Jacobi iteration](../../../../../weighted-jacobi-method.md) with weight $4/5$, to damp grid-scale oscillations in the error.
- Form the fine-grid [linear-system residual](../../../../../linear-system-residual.md) $r_h=f_h-A_hu_h$ and restrict it to the grid of spacing $2h$. An example is the [full-weighting restriction](../../../../../full-weighting-restriction.md) stencil $\tfrac1{16}\left(\begin{smallmatrix}1&2&1\\2&4&2\\1&2&1\end{smallmatrix}\right)$, centered at a coarse-grid point.
- Solve the coarse error equation $A_{2h}e_{2h}=Rr_h$, with homogeneous error boundary data. The [coarse-grid operator](../../../../../coarse-grid-operator.md) may be the rediscretized Poisson operator at spacing $2h$, or the [Galerkin coarse-grid operator](../../../../../galerkin-coarse-grid-operator.md) $A_{2h}=RA_hP$ with consistent transfer operators.
- Prolong the correction to the fine grid, for example by [bilinear interpolation](../../../../../bilinear-interpolation.md), and update $u_h\leftarrow u_h+Pe_{2h}$.
- Apply a few further smoothing sweeps to damp oscillatory components introduced by interpolation.

The coarse solve is performed recursively, with a direct solve on the smallest grid, giving a V-cycle. Smoothing treats oscillations that are cheap for local relaxation to remove; coarse-grid correction treats errors that appear smooth on the fine grid. The scaling of the residual and coarse operator must agree if one instead uses the paper's unscaled stencil.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [3](../../3.md)
3. [A](../../../a.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../split.md)
6. [Numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../../numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

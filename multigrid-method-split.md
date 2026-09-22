# Multigrid method

↑ **Parent:** [Numerical analysis](numerical-analysis-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Multigrid_method)

A [multigrid method](multigrid-method-split.md) solves a [linear system](system-of-linear-equations.md) by combining local relaxation with [coarse-grid correction](coarse-grid-correction.md) on a hierarchy of [meshes](finite-element-mesh.md). The key is to divide the work by scale: a suitable relaxation removes rapidly oscillating [approximation error](approximation-error.md), while [coarse-grid correction](coarse-grid-correction.md) addresses slowly varying [approximation error](approximation-error.md) that relaxation barely changes. A broad error hump occupies many fine-grid points but fewer coarse-grid points; it becomes easier to resolve by relaxation after enough coarsening. This complementary action is why [multigrid methods](multigrid-method-split.md) are useful for large [finite difference method](finite-difference-method.md) and [finite element method](finite-element-method-split.md) systems.

For a concrete model, take the one-dimensional [Poisson equation](poisson-s-equation.md) with homogeneous [Dirichlet boundary conditions](dirichlet-boundary-condition.md):

$$
-u''(x)=f(x),\qquad 0<x<1,\qquad u(0)=u(1)=0.
$$

Use $n$ interior points $x_j=jh$, $h=1/(n+1)$, and the centered [finite difference](finite-difference-split.md) system

$$
(A_hu_h)_j=\frac{2u_{h,j}-u_{h,j-1}-u_{h,j+1}}{h^2}=b_{h,j},\qquad b_{h,j}=f(x_j),\qquad u_{h,0}=u_{h,n+1}=0.
$$

Thus $A_h=h^{-2}\operatorname{tridiag}(-1,2,-1)$ is a [symmetric matrix](symmetric-matrix.md) and a [positive-definite matrix](positive-definite-matrix.md). The minus sign in $-u''$ fixes this positive convention; changing both $A_h$ and $b_h$ to their negatives leaves the relaxation update unchanged. For $f=1$, the [linear system](system-of-linear-equations.md) has the exact discrete solution $u_{h,j}=x_j(1-x_j)/2$, since the centered [finite difference](finite-difference-split.md) is exact on this [quadratic polynomial](quadratic-polynomial.md). In general, the exact discrete solution need not equal the sampled continuous solution: solving the [linear system](system-of-linear-equations.md) removes algebraic [approximation error](approximation-error.md), not the [global discretization error](global-discretization-error.md).

Let $u_h^*$ solve $A_hu_h^*=b_h$, let $v_h$ be the current approximation, and define the signed [approximation error](approximation-error.md) $e_h=u_h^*-v_h$. The [linear-system residual](linear-system-residual.md) is $r_h=b_h-A_hv_h$, so $A_he_h=r_h$. In particular, a [linear-system residual](linear-system-residual.md) is available without knowing $u_h^*$; it supplies the right-hand side for a correction equation. With $D=2h^{-2}I$, a [weighted Jacobi method](weighted-jacobi-method.md) sweep is

$$
v_h\leftarrow v_h+\omega D^{-1}r_h,\qquad e_h\leftarrow S_\omega e_h,\qquad S_\omega=I-\omega D^{-1}A_h.
$$

The [sine](sine.md) [eigenvectors](eigenvector.md) shared by $A_h$ and the [iteration matrix](iteration-matrix.md) $S_\omega$ are $w_j^{(k)}=\sin(k\pi j/(n+1))$, $1\leq k\leq n$. Their [eigenvalues](eigenvalue.md) are

$$
\lambda_k(A_h)=4h^{-2}\sin^2\frac{k\pi}{2(n+1)},\qquad \mu_k(S_\omega)=1-2\omega\sin^2\frac{k\pi}{2(n+1)}.
$$

For $n=63$, one [weighted Jacobi method](weighted-jacobi-method.md) sweep with $\omega=2/3$ multiplies the lowest [Fourier frequency](fourier-frequency.md) mode $k=1$ by about $0.999197$, but the highest [Fourier frequency](fourier-frequency.md) mode $k=63$ by about $-0.332530$. Four sweeps retain about $99.68\%$ of the first amplitude and $1.22\%$ of the second. The sign reversal of the second amplitude is harmless when its magnitude shrinks. However, the plain [Jacobi method](jacobi-method.md), $\omega=1$, has factor $\cos(k\pi/(n+1))$: at $k=63$ it is about $-0.998795$. A nearly alternating mode near the grid's Nyquist limit therefore persists almost as strongly as the smoothest mode. Plain [Jacobi method](jacobi-method.md) convergence on a fixed [Dirichlet boundary condition](dirichlet-boundary-condition.md) grid does not imply effective smoothing.[Introduction to Multigrid Methods by Long Chen](introduction-to-multigrid-methods-by-long-chen.md) The [high-frequency smoothing factor of weighted Jacobi](high-frequency-smoothing-factor-of-weighted-jacobi.md) is uniformly at most $1/3$ for $\omega=2/3$ and $k\geq(n+1)/2$; the [exact finite-grid high-frequency Jacobi smoothing optimum](exact-finite-grid-high-frequency-jacobi-smoothing-optimum.md) distinguishes this convenient uniform choice from the finite-grid optimum.[CS267: Supplemental Notes for Lecture 17 — How Multigrid Damps High Frequencies by James Demmel](cs267-supplemental-notes-for-lecture-17-how-multigrid-damps-high-frequencies-by-james-demmel.md)

<a id="image-analytic-poisson-error-modes-weighted-jacobi-damps-short-wavelengths-while-plain-jacobi-struggles-near-the-nyquist-limit"></a>
![](multigrid-coarse-grid-smoothing.png)

**[Figure 1](#image-analytic-poisson-error-modes-weighted-jacobi-damps-short-wavelengths-while-plain-jacobi-struggles-near-the-nyquist-limit). Analytic Poisson error modes: weighted Jacobi damps short wavelengths while plain Jacobi struggles near the Nyquist limit**.

One two-grid cycle applies a few [weighted Jacobi method](weighted-jacobi-method.md) sweeps, computes the [linear-system residual](linear-system-residual.md), performs [coarse-grid correction](coarse-grid-correction.md), and applies a few more sweeps. The first relaxation makes the remaining [approximation error](approximation-error.md) easier to represent on a coarse [mesh](finite-element-mesh.md); the last relaxation damps oscillatory components left after the transferred correction. In a [geometric multigrid V-cycle](geometric-multigrid-v-cycle.md), replace the expensive exact coarse solve by one recursive cycle on the coarse correction equation, starting its correction from zero. Repeat until a tiny coarsest [linear system](system-of-linear-equations.md) can be solved directly, then return through the levels by adding each interpolated correction and post-smoothing. The descent and return give the cycle its V shape.[slides 59–63](a-multigrid-tutorial-lecture-slides-by-william-l-briggs.md)

For this one-dimensional model, fixed sweep counts and bounded local [finite difference](finite-difference-split.md) and transfer work give a [geometric multigrid V-cycle](geometric-multigrid-v-cycle.md) cost proportional to $n+n/2+n/4+\cdots<2n$, hence $O(n)$ in [Big O notation](big-o-notation.md). A fixed error reduction also needs a contraction factor bounded below one independently of $h$; per-cycle work alone does not establish that. Starting from arbitrary [approximation error](approximation-error.md) and demanding a relative reduction $\varepsilon$ generally adds a factor proportional to $\log(1/\varepsilon)$ in the cycle count. [Full multigrid](full-multigrid.md) uses coarse solutions as initial guesses on successively finer [meshes](finite-element-mesh.md) to target the [global discretization error](global-discretization-error.md) efficiently. The [two-grid Poisson factor with weighted Jacobi](two-grid-poisson-factor-with-weighted-jacobi.md) illustrates favorable convergence for this model. Other [partial differential equations](partial-differential-equation-split.md), strong [anisotropy](anisotropy.md), or poorly chosen coarse spaces and relaxation can defeat these choices; a linear-work guarantee for arbitrary [linear systems](system-of-linear-equations.md) does not follow.

A historical example of the multilevel viewpoint is Achi Brandt's April 1977 paper, which analyzes adaptive [meshes](finite-element-mesh.md) and reports numerical experiments on linear and nonlinear [boundary value problems](boundary-value-problem-split.md). This is a documented development of the approach, not a claim that the paper was its first invention.[pp. 333–390; abstract](multi-level-adaptive-solutions-to-boundary-value-problems-by-achi-brandt.md) The figure above is generated from the displayed [eigenvalues](eigenvalue.md), with lines joining discrete nodes; it contains no experimental measurements.

**Table of contents**

- [Full multigrid](full-multigrid.md)
- [Two-grid Poisson factor with weighted Jacobi](two-grid-poisson-factor-with-weighted-jacobi.md)
- [Geometric multigrid V-cycle](geometric-multigrid-v-cycle.md)
- [Full-weighting restriction](full-weighting-restriction.md)
- [Coarse-grid correction](coarse-grid-correction.md)
  - [Galerkin coarse-grid operator](galerkin-coarse-grid-operator.md)

## ↑ Ancestors (5)

1. [Numerical analysis](numerical-analysis-split.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (8)

- [Coarse-grid correction](coarse-grid-correction.md)
- [Gauss-Seidel method](gauss-seidel-method.md)
- [Jacobi method](jacobi-method.md)
- [Multigrid method](multigrid-method-split.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-67/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-67/7/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-2/37e/b/solution.md)
- [Weighted Jacobi method for the one-dimensional Poisson equation](weighted-jacobi-method-for-the-one-dimensional-poisson-equation.md)

# Finite element method

↑ **Parent:** [Numerical analysis](numerical-analysis-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Finite_element_method)

The [finite element method](finite-element-method.md) replaces an infinite-dimensional [weak formulation](weak-formulation.md) by finitely many unknowns attached to a [finite element mesh](finite-element-mesh.md). Simple local functions, often [piecewise polynomial functions](piecewise-polynomial-function.md), join to form a global approximation. The attraction is that each [finite element](finite-element.md) can be integrated separately, while the assembled equations enforce a global balance. A [piecewise-linear hat function](piecewise-linear-hat-function.md) only meets its immediate neighbors, so a large problem can have a [sparse matrix](sparse-matrix.md) rather than a dense one. Gilbert Strang's MIT lecture develops this connection from the one-dimensional [weak formulation](weak-formulation.md) through local hats to the [stiffness matrix](stiffness-matrix.md) and load integrals.[Gilbert Strang, MIT 18.085, Lecture 18: Finite Elements in 1D, transcript pp. 2–8, 2008; accessed 2026-10-11](https://ocw.mit.edu/courses/18-085-computational-science-and-engineering-i-fall-2008/676ba0a00eef45a6cb3823c4da61ee11_18-085F08-L18.pdf)

For the conforming [Galerkin method](galerkin-method.md), let $V$ be a real [Hilbert space](hilbert-space-split.md), $a$ a bounded [coercive bilinear form](coercive-bilinear-form.md), and $\ell$ a bounded [linear functional](linear-functional.md). Given a [conforming finite element space](conforming-finite-element-space.md) $V_h\subset V$, the continuous and discrete problems are

$$
\begin{aligned}
u\in V:&\quad a(u,v)=\ell(v)&&\text{for every }v\in V,\\
u_h\in V_h:&\quad a(u_h,v_h)=\ell(v_h)&&\text{for every }v_h\in V_h.
\end{aligned}
$$

Writing $u_h=\sum_j c_j\phi_j$ in a [basis](basis.md) of $V_h$ gives the [linear system](system-of-linear-equations.md)

$$
Kc=F,\qquad K_{ij}=a(\phi_j,\phi_i),\qquad F_i=\ell(\phi_i).
$$

Here $K$ is the [stiffness matrix](stiffness-matrix.md) and $F$ is the vector of loads tested against the [basis](basis.md) functions. The [Galerkin method](galerkin-method.md) uses the same trial and test space in this construction. Finite element methods also use the [Petrov-Galerkin method](petrov-galerkin-method.md), with different trial and test spaces; testing against the trial space is therefore a property of this construction, rather than a definition of every [finite element method](finite-element-method.md).

The [finite element solution of the one-dimensional Poisson equation](finite-element-solution-of-the-one-dimensional-poisson-equation.md) below gives every entry explicitly. Refining the [finite element mesh](finite-element-mesh.md) then improves the approximation by adding local degrees of freedom. For a symmetric [coercive bilinear form](coercive-bilinear-form.md), [Galerkin orthogonality](galerkin-orthogonality.md) makes the discrete solution the best approximation in the [energy norm](energy-norm.md); the geometry of [orthogonal projection](orthogonal-projection.md) explains why this local construction yields a globally meaningful answer.

**Table of contents**

- [Finite element solution of the one-dimensional Poisson equation](finite-element-solution-of-the-one-dimensional-poisson-equation.md)
- [Semidiscrete finite element heat equation](semidiscrete-finite-element-heat-equation.md)
  - [Forward Euler limit for a consistent hat mass matrix](forward-euler-limit-for-a-consistent-hat-mass-matrix.md)
- [Finite element](finite-element.md)
- [Conforming finite element space](conforming-finite-element-space.md)
- [Finite element mesh](finite-element-mesh.md)
  - [Shape-regular mesh](shape-regular-mesh.md)
- [Finite element interpolation estimate](finite-element-interpolation-estimate.md)
- [Mass matrix](mass-matrix.md)
  - [Mass eigenstate](mass-eigenstate.md)
  - [Affine-weighted hat mass matrix](affine-weighted-hat-mass-matrix.md)
- [Stiffness matrix](stiffness-matrix.md)
  - [Reaction-diffusion finite element matrix](reaction-diffusion-finite-element-matrix.md)
- [Energy conservation for semidiscrete Galerkin advection](energy-conservation-for-semidiscrete-galerkin-advection.md)
- [Cubic Hermite finite element](cubic-hermite-finite-element.md)
- [Rayleigh-Ritz method](rayleigh-ritz-method.md)
  - [Ritz-Galerkin equivalence for a symmetric coercive form](ritz-galerkin-equivalence-for-a-symmetric-coercive-form.md)
    - [Symmetry and coercivity in quadratic energy minimization](symmetry-and-coercivity-in-quadratic-energy-minimization.md)
  - [Energy norm](energy-norm.md)
- [Galerkin orthogonality](galerkin-orthogonality.md)
  - [Céa's lemma](cea-s-lemma.md)
    - [Aubin–Nitsche duality argument](aubin-nitsche-duality-argument.md)
- [Piecewise-linear hat function](piecewise-linear-hat-function.md)

## ↑ Ancestors (5)

1. [Numerical analysis](numerical-analysis-split.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (7)

- [Finite element method](finite-element-method.md)
- [Finite element solution of the one-dimensional Poisson equation](finite-element-solution-of-the-one-dimensional-poisson-equation.md)
- [Multigrid method](multigrid-method.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-80/5/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-72/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-66/7/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-341/6/solution.md)

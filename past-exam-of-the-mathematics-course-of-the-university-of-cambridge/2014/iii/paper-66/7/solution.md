<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

The [finite element method](../../../../../finite-element-method.md) replaces an infinite-dimensional variational problem by a finite-dimensional one, usually using functions that are polynomial on small mesh elements. [Ritz method](../../../../../rayleigh-ritz-method.md) and [Galerkin method](../../../../../galerkin-method.md) describe how the discrete equations are selected; neither intrinsically requires piecewise polynomials, though those spaces make assembly local and sparse.

For a concrete realization of the two-point problem, choose homogeneous [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md) at both endpoints of $(0,1)$. The differential expression alone is not a complete boundary value problem, so this boundary choice is an explicit assumption. Let $p\in W^{1,\infty}$ with $p\geq p_0>0$, $q\in L^\infty$ with $q\geq0$, and $f\in L^2$. Use the [zero-boundary Sobolev space](../../../../../zero-boundary-sobolev-space.md) $V=H_0^1(0,1)$ with norm $\|v\|_V=\|v'\|_2$. By the [Poincaré inequality](../../../../../poincare-inequality.md) this is equivalent to its full first-order Sobolev norm. Multiplying by a test function and applying [integration by parts](../../../../../integration-by-parts.md) gives

$$
a(u,v)=\ell(v)\quad(v\in V),\qquad
a(u,v)=\int_0^1(pu'v'+quv)\,dx,\quad
\ell(v)=\int_0^1fv\,dx.
$$

The endpoint terms vanish by the essential boundary condition. The form is a [symmetric bilinear form](../../../../../symmetric-bilinear-form.md), bounded by

$$
|a(u,v)|\leq M\|u\|_V\|v\|_V,\qquad
M=\|p\|_\infty+C_P^2\|q\|_\infty,
$$

and it is a [coercive bilinear form](../../../../../coercive-bilinear-form.md):

$$
a(v,v)\geq p_0\|v\|_V^2.
$$

The load is a bounded linear functional. The [Lax-Milgram theorem](../../../../../lax-milgram-theorem.md) gives a unique weak solution and a bound $\|u\|_V\leq\|\ell\|_{V^*}/p_0$. Under the stated coefficient regularity it solves the differential equation in the usual weak sense.

The [Ritz method](../../../../../rayleigh-ritz-method.md) minimizes the energy

$$
J(v)=\tfrac12a(v,v)-\ell(v)
$$

over $V$, or over a conforming finite-dimensional subspace $V_h\subset V$. Its first variation is $a(v,w)-\ell(w)$; symmetry and coercivity make the functional strictly convex. In fact, if $u$ is the weak solution,

$$
J(v)-J(u)=\tfrac12a(v-u,v-u)\geq0.
$$

Thus the energy minimizer is exactly the weak solution. The [Galerkin method](../../../../../galerkin-method.md) instead directly asks for $u_h\in V_h$ with $a(u_h,v_h)=\ell(v_h)$ for all $v_h\in V_h$. For this symmetric coercive problem, [Ritz-Galerkin equivalence for a symmetric coercive form](../../../../../ritz-galerkin-equivalence-for-a-symmetric-coercive-form.md) shows that the discrete minimizer and Galerkin solution coincide. For a nonsymmetric problem, a Galerkin formulation can still apply but the same quadratic minimization generally cannot represent its full [bilinear form](../../../../../bilinear-form.md); appropriate coercivity or inf-sup conditions must then justify the chosen spaces.

Subtract the continuous and discrete weak equations to obtain [Galerkin orthogonality](../../../../../galerkin-orthogonality.md) $a(u-u_h,v_h)=0$. Since $a$ defines the [energy norm](../../../../../energy-norm.md) $\|v\|_a=\sqrt{a(v,v)}$, the [Pythagorean identity](../../../../../pythagorean-theorem-in-an-inner-product-space.md) gives

$$
\|u-v_h\|_a^2=\|u-u_h\|_a^2+\|u_h-v_h\|_a^2,
\qquad
\boxed{\|u-u_h\|_a=\inf_{v_h\in V_h}\|u-v_h\|_a.}
$$

In a general reference norm, the [Céa lemma](../../../../../cea-s-lemma.md) yields

$$
\boxed{\|u-u_h\|_V\leq\frac{M}{p_0}
\inf_{v_h\in V_h}\|u-v_h\|_V.}
$$

The proof uses $a(e,e)=a(e,u-v_h)$ together with coercivity and continuity. Dense approximation spaces therefore imply convergence; the estimate reduces a numerical error problem to an approximation problem.

For implementation, partition the interval by nodes $0=x_0<\cdots<x_N=1$. Choose continuous piecewise-linear functions and the interior [piecewise-linear hat functions](../../../../../piecewise-linear-hat-function.md) $\phi_j$ as a basis, with the two boundary coefficients prescribed. Write $u_h=\sum_jU_j\phi_j$. The coefficients satisfy

$$
\boxed{KU=F,\qquad K_{ij}=\int_0^1(p\phi_j'\phi_i'+q\phi_j\phi_i)\,dx,
\quad F_i=\int_0^1f\phi_i\,dx.}
$$

The [stiffness matrix](../../../../../stiffness-matrix.md) is symmetric positive definite: $U^TKU=a(u_h,u_h)>0$ for nonzero interior coefficients. The local supports make it tridiagonal in this one-dimensional linear-element case.

On an element of length $h_e$, for constant element coefficients $p_e,q_e$, the two-node [matrix](../../../../../matrix.md) and constant-load vector are

$$
K_e=\frac{p_e}{h_e}
\begin{pmatrix}1&-1\\-1&1\end{pmatrix}
+\frac{q_eh_e}{6}
\begin{pmatrix}2&1\\1&2\end{pmatrix},
\qquad
F_e=\frac{f_eh_e}{2}\begin{pmatrix}1\\1\end{pmatrix}.
$$

For variable coefficients, integrate $p,q,f$ against the same shape functions rather than silently replacing them by constants. Element contributions are added at shared nodes, and boundary values are eliminated or lifted into the right side. A sparse direct solve or a suitable iterative method gives the nodal coefficients. Numerical quadrature should preserve the required accuracy and, with positive coefficients and weights, the positive energy structure.

A [finite element interpolation estimate](../../../../../finite-element-interpolation-estimate.md) gives $\inf_{v_h}\|u-v_h\|_{H^1}\leq Ch\|u\|_{H^2}$ for these elements, where $h$ is the largest element size and the solution has the stated regularity. The [Céa lemma](../../../../../cea-s-lemma.md) then gives **first-order energy error**. If the dual elliptic problem has $H^2$ regularity, the [Aubin–Nitsche duality argument](../../../../../aubin-nitsche-duality-argument.md) gives **second-order $L^2$ error**: for $e=u-u_h$, solve $a(v,z)=(e,v)_{L^2}$, then use $a(e,z)=a(e,z-I_hz)$ to gain one further factor of $h$. Higher-order elements improve rates when the solution is sufficiently smooth.

Nonzero Dirichlet data are handled by a boundary lifting and an affine trial space. [Neumann boundary conditions](../../../../../neumann-boundary-condition.md) enter naturally through the integrated boundary term; Robin terms modify both the form and the load. With pure Neumann conditions and $q=0$, constants lie in the kernel: existence needs the load/flux compatibility condition, uniqueness needs a mean constraint, and the preceding Dirichlet coercivity argument cannot simply be reused. **Conforming approximation, boundary conditions and coercivity are the ingredients connecting the finite-element construction to a justified Ritz or Galerkin solution.**

## ↑ Ancestors (10)

1. [7](../7.md)
2. [Paper 66](../../paper-66-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

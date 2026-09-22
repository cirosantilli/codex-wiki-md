<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

Consider a bounded [Lipschitz domain](../../../../../lipschitz-domain.md) $\Omega$ and homogeneous [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md) for

$$
-\nabla\cdot(A(x)\nabla u)+c(x)u=f.
$$

Assume $A$ is a bounded real [symmetric matrix](../../../../../symmetric-matrix.md) field with $\xi^TA(x)\xi\geq a_0|\xi|^2$ uniformly, $c\geq0$ is bounded, and $f$ defines a bounded linear functional on $V=H_0^1(\Omega)$, the [zero-boundary Sobolev space](../../../../../zero-boundary-sobolev-space.md). The [weak formulation](../../../../../weak-formulation.md) is

$$
a(u,v)=\ell(v)\quad(v\in V),\qquad
 a(u,v)=\int_\Omega\nabla v^TA\nabla u+cuv,\quad\ell(v)=\langle f,v\rangle.
$$

The [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) gives continuity $|a(u,v)|\leq M\|u\|_V\|v\|_V$. Uniform ellipticity and the [Poincaré inequality](../../../../../poincare-inequality.md) give a [coercive bilinear form](../../../../../coercive-bilinear-form.md), $a(v,v)\geq\alpha\|v\|_V^2$. The [Lax-Milgram theorem](../../../../../lax-milgram-theorem.md) therefore supplies a unique [weak solution](../../../../../weak-solution.md), with $\|u\|_V\leq\|\ell\|_{V'}/\alpha$. Its proof represents $a$ by a [bounded linear operator](../../../../../continuous-linear-operator.md) $T$ using the [Riesz representation theorem](../../../../../riesz-representation-theorem.md); coercivity gives an injective operator with closed image, and a zero [orthogonal complement](../../../../../orthogonal-complement.md) makes that image all of $V$. This yields existence, uniqueness and the displayed estimate.

For a [conforming finite element space](../../../../../conforming-finite-element-space.md) $V_h\subseteq V$, the [Galerkin method](../../../../../galerkin-method.md) finds $u_h\in V_h$ such that $a(u_h,v_h)=\ell(v_h)$ for every $v_h\in V_h$. With a basis $\phi_1,\ldots,\phi_N$, this is the linear system $KU=F$, where the [stiffness matrix](../../../../../stiffness-matrix.md) is $K_{ij}=a(\phi_j,\phi_i)$ and $F_i=\ell(\phi_i)$. Its [positive-definite matrix](../../../../../positive-definite-matrix.md) property proves unique discrete solvability. Local support gives a [sparse matrix](../../../../../sparse-matrix.md) through elementwise assembly.

For the symmetric problem, the [Ritz method](../../../../../rayleigh-ritz-method.md) minimizes $J(v)=a(v,v)/2-\ell(v)$ over $V_h$. Differentiating in every direction $v_h$ gives precisely the [Galerkin method](../../../../../galerkin-method.md) equations. Conversely, if $u_h$ solves them, $J(u_h+w_h)-J(u_h)=a(w_h,w_h)/2$, proving it is the unique minimum. The same argument over $V$ gives $J(v)-J(u)=\|v-u\|_a^2/2$, where $\|v\|_a=\sqrt{a(v,v)}$ is the [energy norm](../../../../../energy-norm.md). Thus the [Ritz method](../../../../../rayleigh-ritz-method.md) chooses the best trial function in that norm.

Subtracting the continuous and discrete equations gives [Galerkin orthogonality](../../../../../galerkin-orthogonality.md), $a(u-u_h,v_h)=0$. For arbitrary $v_h\in V_h$ and $e=u-u_h$, it follows that $a(e,e)=a(e,u-v_h)$. Coercivity and continuity prove the [Céa lemma](../../../../../cea-s-lemma.md):

$$
\alpha\|e\|_V^2\leq M\|e\|_V\|u-v_h\|_V,
\qquad
\|u-u_h\|_V\leq\frac M\alpha\inf_{v_h\in V_h}\|u-v_h\|_V.
$$

In the symmetric [energy norm](../../../../../energy-norm.md), the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) improves the constant to one. Equivalently, [Galerkin orthogonality](../../../../../galerkin-orthogonality.md) gives the [Pythagorean identity](../../../../../pythagorean-theorem-in-an-inner-product-space.md) $\|u-v_h\|_a^2=\|u-u_h\|_a^2+\|u_h-v_h\|_a^2$. These estimates establish stability and show that approximation properties of the trial space determine convergence.

For continuous piecewise-linear elements on a [shape-regular mesh](../../../../../shape-regular-mesh.md) in dimensions at most three, a [finite element interpolation estimate](../../../../../finite-element-interpolation-estimate.md) gives $\|u-I_hu\|_{H^1}\leq Ch\|u\|_{H^2}$ when $u\in H^2(\Omega)$. Combining it with the [Céa lemma](../../../../../cea-s-lemma.md) yields $O(h)$ [energy norm](../../../../../energy-norm.md) error. More generally, degree-$p$ elements give $O(h^p)$ error in $H^1$ under the corresponding regularity and approximation assumptions. Mere mesh refinement cannot supply an order whose required solution regularity is absent.

An additional order in the [L2 norm](../../../../../l2-norm.md) follows under a dual [elliptic regularity](../../../../../elliptic-regularity.md) assumption. Solve $a(v,z)=(e,v)_{L^2}$ and assume $\|z\|_{H^2}\leq C\|e\|_{L^2}$. The [Aubin–Nitsche duality argument](../../../../../aubin-nitsche-duality-argument.md) uses [Galerkin orthogonality](../../../../../galerkin-orthogonality.md) to obtain

$$
\|e\|_{L^2}^2=a(e,z-I_hz)\leq Ch\|e\|_{H^1}\|z\|_{H^2}
\leq Ch\|e\|_{H^1}\|e\|_{L^2}.
$$

Therefore $\|e\|_{L^2}\leq Ch\|e\|_{H^1}$, giving $O(h^2)$ for the piecewise-linear case with $u\in H^2$. This improvement explicitly requires regularity of the dual problem.

As a concrete example, solve $-u''=1$ on $(0,1)$ with zero endpoint values. On a uniform mesh of spacing $h$, the [piecewise-linear hat functions](../../../../../piecewise-linear-hat-function.md) give $K_{jj}=2/h$, $K_{j,j\pm1}=-1/h$ and $F_j=h$. The discrete equations are $2U_j-U_{j-1}-U_{j+1}=h^2$, whose solution is $U_j=x_j(1-x_j)/2$. The exact solution is $u(x)=x(1-x)/2$, so $u_h$ is its piecewise-linear nodal interpolant. On each interval $[x_j,x_{j+1}]$,

$$
u-u_h=\frac12(x-x_j)(x_{j+1}-x).
$$

Integrating the squared error and squared derivative error gives the explicit rates

$$
\boxed{\|u-u_h\|_{H_0^1}=\frac h{\sqrt{12}},\qquad\|u-u_h\|_{L^2}=\frac{h^2}{\sqrt{120}},}
$$

where the $H_0^1$ norm here is $\|v'\|_{L^2}$.

For nonsymmetric coercive problems, the [Galerkin method](../../../../../galerkin-method.md), [Galerkin orthogonality](../../../../../galerkin-orthogonality.md) and the [Céa lemma](../../../../../cea-s-lemma.md) still apply, but the symmetric quadratic minimization interpretation of the [Ritz method](../../../../../rayleigh-ritz-method.md) generally does not. Nonconforming trial spaces, inexact integration and noncoercive equations need additional arguments beyond the conforming coercive theory proved here.

## ↑ Ancestors (10)

1. [7](../7.md)
2. [Paper 341](../../paper-341-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

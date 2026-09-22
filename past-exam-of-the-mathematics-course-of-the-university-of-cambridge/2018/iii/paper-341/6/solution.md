<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

The starting point of a conforming [finite element method](../../../../../finite-element-method.md) is a [weak formulation](../../../../../weak-formulation.md) in a [Hilbert space](../../../../../hilbert-space-split.md) $X$. For example, a homogeneous [Dirichlet boundary condition](../../../../../dirichlet-boundary-condition.md) on a bounded [Lipschitz domain](../../../../../lipschitz-domain.md) gives $X=H_0^1(\Omega)$. One seeks

$$
a(u,v)=\ell(v)\qquad(v\in X),
$$

where $a$ is a [bounded bilinear form](../../../../../bounded-bilinear-form.md), $|a(w,v)|\leq L\|w\|_X\|v\|_X$, and $\ell\in X^*$ is a bounded [linear functional](../../../../../linear-functional.md). A [conforming finite element space](../../../../../conforming-finite-element-space.md) $X_h\subset X$ is finite dimensional and is typically built from functions that are polynomial on each element of a [finite element mesh](../../../../../finite-element-mesh.md). With a basis $\varphi_j$, the [Galerkin method](../../../../../galerkin-method.md) imposes the same identity only for $v_h\in X_h$, giving

$$
\boxed{Kc=F,\qquad K_{ij}=a(\varphi_j,\varphi_i),\quad F_i=\ell(\varphi_i).}
$$

The [stiffness matrix](../../../../../stiffness-matrix.md) is sparse when basis supports overlap only locally. Local element integrals assemble its entries; the [mass matrix](../../../../../mass-matrix.md) represents an $L^2$ term. This separates the choice of trial functions from the variational principle determining their coefficients.

The fundamental well-posedness theorem is the [Lax-Milgram theorem](../../../../../lax-milgram-theorem.md): if $a(v,v)\geq\gamma\|v\|_X^2$ for some $\gamma>0$, there is a unique solution for each $\ell\in X^*$, with $\|u\|_X\leq\|\ell\|_{X^*}/\gamma$. The same theorem on $X_h$ gives a unique discrete solution. The constants must be independent of the mesh for uniform [stability of a numerical method](../../../../../stability-of-a-numerical-method.md). Boundary conditions are built into the trial space when they are essential constraints; flux conditions arise through boundary terms in [integration by parts](../../../../../integration-by-parts.md) and are natural constraints in the [weak formulation](../../../../../weak-formulation.md).

When $a$ is symmetric and a [coercive bilinear form](../../../../../coercive-bilinear-form.md), the [Ritz method](../../../../../rayleigh-ritz-method.md) minimizes

$$
\mathcal E(v)=\tfrac12a(v,v)-\ell(v)
$$

over $X_h$. Its first variation is exactly the [Galerkin method](../../../../../galerkin-method.md), so **Ritz minimization and Galerkin testing coincide for symmetric coercive problems**. The [energy norm](../../../../../energy-norm.md) $\|v\|_a=\sqrt{a(v,v)}$ turns the approximation into an [orthogonal projection](../../../../../orthogonal-projection.md). Indeed, subtracting the exact and discrete weak equations gives [Galerkin orthogonality](../../../../../galerkin-orthogonality.md), $a(u-u_h,v_h)=0$. For every $v_h\in X_h$ the [Pythagorean identity](../../../../../pythagorean-theorem-in-an-inner-product-space.md) becomes

$$
\|u-v_h\|_a^2=\|u-u_h\|_a^2+\|u_h-v_h\|_a^2,
$$

so

$$
\boxed{\|u-u_h\|_a=\inf_{v_h\in X_h}\|u-v_h\|_a.}
$$

This exact best-approximation property is the central advantage of the [Ritz method](../../../../../rayleigh-ritz-method.md).

Symmetry is unnecessary for the [Galerkin method](../../../../../galerkin-method.md). For any bounded, coercive form, the [Céa lemma](../../../../../cea-s-lemma.md) gives

$$
\boxed{\|u-u_h\|_X\leq\frac L\gamma
\inf_{v_h\in X_h}\|u-v_h\|_X.}
$$

To prove it, put $e=u-u_h$. [Galerkin orthogonality](../../../../../galerkin-orthogonality.md) yields $a(e,e)=a(e,u-v_h)$, so coercivity and boundedness give $\gamma\|e\|_X^2\leq L\|e\|_X\|u-v_h\|_X$. Divide when $e\neq0$ and take the [infimum](../../../../../infimum.md). Thus approximation capability plus uniform coercivity gives convergence. In contrast, minimizing $\tfrac12a(v,v)-\ell(v)$ for a nonsymmetric form differentiates its symmetric part and generally does not solve the original weak equation.

A concrete symmetric example is the one-dimensional reaction-diffusion problem from Question 5. Continuous [piecewise-linear hat functions](../../../../../piecewise-linear-hat-function.md) give the diffusion [stiffness matrix](../../../../../stiffness-matrix.md) $S$ with diagonal $2/h$ and neighbouring entries $-1/h$, and the [mass matrix](../../../../../mass-matrix.md) $M$ with diagonal $2h/3$ and neighbouring entries $h/6$. Therefore $K=S+M$ and $F_i=ih^2$. Its [positive-definite matrix](../../../../../positive-definite-matrix.md) is the coordinate form of the continuous energy. The exact smooth solution $u(x)=x-\sinh(x)/\sinh1$ makes this an explicit test of the method, not just an abstract existence result.

For a nonsymmetric example, take positive $\varepsilon$, constant real $\beta$, and

$$
-\varepsilon u''+\beta u'+u=f,\qquad u(0)=u(1)=0.
$$

Its form is $a(u,v)=\varepsilon\int u'v'+\beta\int u'v+\int uv$. Since $\int v'v=0$, it has coercivity constant $\min(\varepsilon,1)$ in the full $H^1$ norm, although it is not symmetric when $\beta\neq0$. The [Galerkin method](../../../../../galerkin-method.md) remains well posed. On the uniform hat basis, $K=\varepsilon S+\beta C+M$, where $C_{i,i+1}=1/2$, $C_{i,i-1}=-1/2$ and $C_{ii}=0$. The [skew-symmetric matrix](../../../../../skew-symmetric-matrix.md) $C$ cancels from $c^TKc$, proving nonsingularity. A Ritz energy would omit precisely this advection contribution. Small $\varepsilon$ may nevertheless make the approximation constant large and produce poorly resolved layers; algebraic solvability is not an accuracy guarantee.

Quantitative convergence uses a [finite element interpolation estimate](../../../../../finite-element-interpolation-estimate.md). On a [shape-regular mesh](../../../../../shape-regular-mesh.md), for piecewise-linear conforming elements and $u\in H^2(\Omega)$ in the usual low-dimensional setting,

$$
\|u-I_hu\|_{H^1}\leq Ch\|u\|_{H^2},\qquad
\|u-I_hu\|_{L^2}\leq Ch^2\|u\|_{H^2}.
$$

The [Céa lemma](../../../../../cea-s-lemma.md) therefore gives an $O(h)$ energy error. The [Aubin–Nitsche duality argument](../../../../../aubin-nitsche-duality-argument.md) improves the [L2 norm](../../../../../l2-norm.md) error when the dual elliptic problem has $H^2$ regularity: solve $a(v,z)=(e,v)_{L^2}$ and use

$$
\|e\|_{L^2}^2=a(e,z-I_hz)
\leq Ch\|e\|_{H^1}\|z\|_{H^2}
\leq Ch\|e\|_{H^1}\|e\|_{L^2}.
$$

Consequently

$$
\boxed{\|u-u_h\|_{H^1}=O(h),\qquad
\|u-u_h\|_{L^2}=O(h^2),}
$$

with constants depending on the solution and regularity bounds. The second estimate is conditional on dual regularity; corners or insufficient data regularity can reduce the rate.

The same [Galerkin method](../../../../../galerkin-method.md) handles evolution equations. For the homogeneous [heat equation](../../../../../heat-equation.md), the [semidiscrete finite element heat equation](../../../../../semidiscrete-finite-element-heat-equation.md) is $M\dot c+Sc=0$. Because $M$ is a [positive-definite matrix](../../../../../positive-definite-matrix.md) and $S$ is a [positive semidefinite matrix](../../../../../positive-semidefinite-matrix.md),

$$
\frac{d}{dt}(c^TMc)=-2c^TSc\leq0.
$$

The decreasing [quadratic form](../../../../../quadratic-form.md) is exactly the [L2 norm](../../../../../l2-norm.md) squared of the finite-element function. This separates spatial [stability of a numerical method](../../../../../stability-of-a-numerical-method.md) from the subsequent time integrator, just as in the [Schrödinger equation](../../../../../schrodinger-equation.md) example. **Conformity, coercivity and approximation estimates together explain convergence.**

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 341](../../paper-341-split.md)
3. [Iii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

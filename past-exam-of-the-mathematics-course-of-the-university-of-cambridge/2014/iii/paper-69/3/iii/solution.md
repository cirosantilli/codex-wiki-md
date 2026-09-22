<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Interpret the printed coordinate notation as the square corners $1+i$, $1-i$, $-1-i$, $-1+i$. This listed order is clockwise, contrary to the counterclockwise convention in (ii). Keep the printed first side directed from top to bottom. Then $m_1=1$, $h_1=-i$, and $z(s)=1-is$. Put $g_1(s)=u(1,-s)$ and $q_1(s)=u_x(1,-s)$, where $q_1$ is the outward [normal derivative](../../../../../../normal-derivative.md) on the right side. The pullback formula, without any orientation shortcut, gives

$$
\boxed{W_1(s,\lambda)=
 e^{-i\beta(\lambda-\lambda^{-1})-\beta s(\lambda+\lambda^{-1})}
 \left[-iq_1(s)+\beta(\lambda-\lambda^{-1})g_1(s)\right].}
$$

Indeed $h_1u_z-\bar h_1u_{\bar z}=-i(u_z+u_{\bar z})=-iu_x$, and $i\beta(\lambda h_1+\bar h_1/\lambda)=\beta(\lambda-\lambda^{-1})$. If one reverses the side to match the counterclockwise convention, its parameter is $1+is$ and its integrand is $-W_1(-s,\lambda)$. Reversing every side multiplies the [global relation](../../../../../../global-relation-for-a-linear-boundary-value-problem.md) by minus one, leaving its zero value unchanged.

**The unheaded numerical reconstruction request.** The four unknown [Neumann boundary conditions](../../../../../../neumann-boundary-condition.md) are four functions on the sides, not four scalar values. The polygonal [global relation](../../../../../../global-relation-for-a-linear-boundary-value-problem.md) is linear in their outward [normal derivatives](../../../../../../normal-derivative.md), and its remaining terms depend only on the prescribed [Dirichlet boundary data](../../../../../../dirichlet-boundary-data.md).

Choose a finite approximation on each side, for example an expansion of $q_j(s)$ in [Legendre polynomials](../../../../../../legendre-polynomial.md) or piecewise polynomials. Substitute those expansions into the consistently oriented [global relation](../../../../../../global-relation-for-a-linear-boundary-value-problem.md). At chosen nonzero [spectral parameters for a linear boundary value problem](../../../../../../spectral-parameter-for-a-linear-boundary-value-problem.md), integrate the exponential kernels against each basis function to assemble a complex linear system; the known right-hand side is obtained by integrating the given [Dirichlet boundary data](../../../../../../dirichlet-boundary-data.md). Use enough independent samples to resolve all side coefficients, and preferably oversample. The [conjugate global relations for the modified Helmholtz equation](../../../../../../conjugate-global-relations-for-the-modified-helmholtz-equation.md) provide useful companion tests; for complex data use the corresponding independent adjoint relation rather than assuming the traces real.

Solve the scaled system by [least-squares solution](../../../../../../least-squares-solution-of-a-linear-inverse-problem.md) using a stable factorization such as a [singular value decomposition](../../../../../../singular-value-decomposition.md). Sampling directions should probe all sides, and exponential row scaling avoids overflow and poor conditioning. Refine the side approximation and spectral samples until the recovered traces and unused [global relation](../../../../../../global-relation-for-a-linear-boundary-value-problem.md) residuals stabilize. Corner incompatibilities or limited corner regularity call for mesh refinement or enriched endpoint basis functions. This realizes a numerical [Dirichlet-to-Neumann map](../../../../../../dirichlet-to-neumann-map.md) without first discretizing the whole interior.

The underlying [Dirichlet problem](../../../../../../dirichlet-problem.md) is uniquely solvable in the usual trace class for $\Delta u-4\beta^2u=0$ with $\beta>0$: the homogeneous problem has $\int_\Omega(|\nabla u|^2+4\beta^2|u|^2)\,dA=0$. This supports the boundary reconstruction, although uniqueness of the continuous problem alone does not guarantee that an arbitrary finite set of spectral samples is well conditioned.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

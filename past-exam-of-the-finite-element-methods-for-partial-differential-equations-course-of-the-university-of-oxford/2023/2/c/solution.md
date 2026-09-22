<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a conforming triangular [finite element mesh](../../../../finite-element-mesh.md), take

$$
V_h=\{v_h\in C^0(\overline\Omega):v_h|_K\in\mathcal P_2(K)\text{ for every }K\in\mathcal M_h,\quad v_h|_{\Gamma_D}=0\}.
$$

This is the quadratic [conforming finite element space](../../../../conforming-finite-element-space.md). Across a common [edge of a polygon](../../../../side-of-a-polygon.md), the restrictions from neighboring [triangles](../../../../triangle.md) are univariate [quadratic polynomials](../../../../quadratic-polynomial.md). Their agreement at the two endpoints and the [midpoint](../../../../midpoint.md) makes their difference a degree-at-most-two [polynomial](../../../../polynomial-split.md) with three distinct [roots of a polynomial](../../../../root-of-a-polynomial.md), so it vanishes on the entire common [edge of a polygon](../../../../side-of-a-polygon.md). Thus matching the local [finite element degrees of freedom](../../../../finite-element-degree-of-freedom.md) produces the required continuity. Similarly, setting the three nodal values on every boundary edge carrying the [Dirichlet boundary condition](../../../../dirichlet-boundary-condition.md) to zero makes its entire restriction vanish.

Continuity across element interfaces means the piecewise [gradients](../../../../gradient.md) give the global [weak gradient](../../../../weak-gradient.md), with no jump contribution, so $V_h\subset V$. There are finitely many local [finite element degrees of freedom](../../../../finite-element-degree-of-freedom.md), hence $V_h$ is finite-dimensional. The [Galerkin method](../../../../galerkin-method.md) seeks

$$
\boxed{u_h\in V_h,\qquad (\nabla u_h,\nabla v_h)_0+(u_h,v_h)_0=(f,v_h)_0\quad(v_h\in V_h).}
$$

The [bounded bilinear form](../../../../bounded-bilinear-form.md) and [coercive bilinear form](../../../../coercive-bilinear-form.md) estimates from part (b) remain valid on $V_h$. Since a [finite-dimensional subspace is closed](../../../../finite-dimensional-subspace-is-closed.md), the [Lax-Milgram theorem](../../../../lax-milgram-theorem.md) gives exactly one $u_h$. Alternatively, the [stiffness matrix](../../../../stiffness-matrix.md) plus the [mass matrix](../../../../mass-matrix.md) is a [positive-definite matrix](../../../../positive-definite-matrix.md) in any [basis](../../../../basis.md) of $V_h$. The same existence and uniqueness conclusion holds for any finite-dimensional [vector subspace](../../../../vector-subspace.md) of this full space.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the finite element methods for partial differential equations course of the University of Oxford](../../../split.md)
5. [Finite element methods for partial differential equations course of the University of Oxford](../../../../finite-element-methods-for-partial-differential-equations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

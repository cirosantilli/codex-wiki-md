<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $e=u-u_h$. Subtracting the two [weak formulations](../../../../weak-formulation.md) gives [Galerkin orthogonality](../../../../galerkin-orthogonality.md), $a(e,v_h)=0$ for every $v_h\in V_h$. Since $a$ is the first-order [Sobolev inner product](../../../../sobolev-inner-product.md), for every $v_h\in V_h$ we have

$$
\begin{aligned}
\|e\|_1^2
&=a(e,u-v_h)+a(e,v_h-u_h)\\
&=a(e,u-v_h)\leq\|e\|_1\|u-v_h\|_1.
\end{aligned}
$$

If $e\ne0$, division proves $\|e\|_1\leq\|u-v_h\|_1$; if $e=0$, the same conclusion is immediate. Thus the [Céa lemma](../../../../cea-s-lemma.md) has constant one in this case.

Use the quadratic nodal [interpolant](../../../../interpolant.md) $I_hu$. The assumed $H^3(\Omega)$ regularity gives continuous nodal values by the [Sobolev embedding theorem](../../../../sobolev-embedding-theorem.md), and its zero [Sobolev trace](../../../../trace-operator.md) makes the nodal values on $\Gamma_D$ zero. The [quadratic Lagrange triangle](../../../../quadratic-lagrange-triangle.md) construction then gives $I_hu\in V_h$. The allowed quadratic [finite element interpolation estimate](../../../../finite-element-interpolation-estimate.md) on a [shape-regular mesh](../../../../shape-regular-mesh.md) is

$$
\|u-I_hu\|_1\leq C_Ih^2\|u\|_{H^3(\Omega)},
$$

where $C_I$ depends on the fixed [triangle](../../../../triangle.md) and [shape regularity](../../../../shape-regular-mesh.md), but not on $h$. Therefore

$$
\boxed{\|u-u_h\|_{H^1(\Omega)}\leq\|u-I_hu\|_{H^1(\Omega)}\leq C_1h^2\|u\|_{H^3(\Omega)},\qquad C_1=C_I.}
$$

This step uses the inclusion $I_hu\in V_h$ explicitly permitted by the question. Arbitrary smaller [vector subspaces](../../../../vector-subspace.md) without the same approximation property would not give this rate.

## ↑ Ancestors (12)

1. [D](../d.md)
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

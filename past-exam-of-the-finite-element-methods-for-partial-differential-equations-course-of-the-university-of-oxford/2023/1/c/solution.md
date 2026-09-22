<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the continuous [piecewise-linear](../../../../piecewise-linear-function.md) nodal [interpolants](../../../../interpolant.md) $I_hu$ and $I_hw$ on the [shape-regular mesh](../../../../shape-regular-mesh.md). Since $u,w\in H^2(\Omega)$ in two dimensions, the [Sobolev embedding theorem](../../../../sobolev-embedding-theorem.md) supplies continuous representatives, so the nodal values are well-defined. Their zero [Sobolev traces](../../../../trace-operator.md) imply zero boundary nodal values. Hence $I_hu\in\mathcal U_h$ and $I_hw\in\mathcal W_h$ for the usual full [conforming finite element spaces](../../../../conforming-finite-element-space.md).

The permitted [finite element interpolation estimates](../../../../finite-element-interpolation-estimate.md) give constants $C_u,C_w$ determined by the [shape regularity](../../../../shape-regular-mesh.md) and $\Omega$, independent of $h$, such that

$$
\|u-I_hu\|_1\leq C_u h\|u\|_{H^2(\Omega)},\qquad
\|w-I_hw\|_1\leq C_w h\|w\|_{H^2(\Omega)}.
$$

Substitute these choices in the [best approximation](../../../../best-approximation-in-a-normed-space.md) bound from part (b):

$$
\boxed{\begin{aligned}
\left(\|u-u_h\|_1^2+\|w-w_h\|_1^2\right)^{1/2}&\leq C_*h,\\
C_*&=(1+K)\left(C_u^2\|u\|_{H^2(\Omega)}^2+C_w^2\|w\|_{H^2(\Omega)}^2\right)^{1/2}.
\end{aligned}}
$$

For fixed $u,w$, this constant is independent of $h$. A [shape-regular mesh](../../../../shape-regular-mesh.md) suffices; no uniformity of the individual element sizes is needed, since $h$ is their maximum diameter.

The inclusion of these [interpolants](../../../../interpolant.md) is an essential assumption. If the wording “consist of” were read as permitting arbitrary smaller [vector subspaces](../../../../vector-subspace.md), taking $\mathcal U_h=\mathcal W_h=\{0\}$ for every $h$ would prevent the claimed convergence for a nonzero solution. The full [conforming finite element space](../../../../conforming-finite-element-space.md) interpretation is also needed for the dimension assertion in part (d).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
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

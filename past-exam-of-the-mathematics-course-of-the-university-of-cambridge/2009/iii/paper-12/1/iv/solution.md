<h1 id="1/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Let $u,v$ be two [critical points](../../../../../../critical-point.md) with the same classical boundary values, and put $w=u-v$. Since $F$ is independent of $z$, the [Euler-Lagrange equation](../../../../../../euler-lagrange-equation.md) for each is $D_iF_{p_i}(x,Du)=0$. By the [fundamental theorem of calculus](../../../../../../fundamental-theorem-of-calculus.md) along the segment between the [gradients](../../../../../../gradient.md),

$$
F_{p_i}(x,Du)-F_{p_i}(x,Dv)=A_{ij}(x)D_jw,\qquad A_{ij}(x)=\int_0^1F_{p_ip_j}(x,Dv+tDw)\,dt.
$$

Subtracting the equations gives $D_i(A_{ij}D_jw)=0$. The [uniformly convex variational integrand](../../../../../../uniformly-convex-variational-integrand.md) makes $A$ symmetric and [uniformly elliptic](../../../../../../uniformly-elliptic-operator.md) with the same positive lower bound. Since $F$ is smooth and $u,v\in C^2(\overline\Omega)$, $A$ is continuously differentiable locally in $\Omega$, so

$$
A_{ij}D_{ij}w+(D_iA_{ij})D_jw=0
$$

is a classical [nondivergence-form elliptic operator](../../../../../../nondivergence-form-elliptic-operator.md) with no zeroth-order term.

To avoid assuming that derivatives of $F$ stay bounded all the way to the boundary, apply the proved [weak maximum principle](../../../../../../weak-maximum-principle-for-elliptic-operators.md) on inner open sets $\Omega_\delta=\{x\in\Omega:\operatorname{dist}(x,\partial\Omega)>\delta\}$. Their closures lie compactly in $\Omega$, so all linearized coefficients there are bounded. The maximum principle applies on each component and yields

$$
\sup_{\Omega_\delta}|w|\leq\sup_{\partial\Omega_\delta}|w|.
$$

Every point of the inner boundary is at distance $\delta$ from $\partial\Omega$. Since $w$ is continuous on the compact closure and equals zero on that boundary, the right-hand side tends uniformly to zero as $\delta\downarrow0$. Every fixed interior point eventually belongs to $\Omega_\delta$, proving

$$
\boxed{u=v\text{ in }\Omega.}
$$

This establishes [uniqueness for uniformly convex gradient Dirichlet problems](../../../../../../uniqueness-for-uniformly-convex-gradient-dirichlet-problems.md) using precisely the boundary continuity and ellipticity needed for the comparison.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [1](../../1.md)
3. [Paper 12](../../../paper-12-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

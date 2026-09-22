<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [Dirichlet uniqueness for the Poisson equation](../../../../dirichlet-uniqueness-for-the-poisson-equation.md) follows from a positive integral. Suppose $T_a,T_b$ satisfy the same data, and put $w=T_a-T_b$. Then $w$ is a [harmonic function](../../../../harmonic-function.md) in $V$ and vanishes on $S$. [Green's first identity](../../../../green-s-first-identity.md), applied with both arguments $w$, gives

$$
\int_V|\nabla w|^2dV=\int_Sw\,\partial_nw\,dS-\int_Vw\Delta w\,dV=0.
$$

Thus $\nabla w=0$, and $w$ is constant on the connected body. Its zero boundary value makes that constant zero. This proves **at most one temperature field**; it does not require an independent existence construction. As usual, the argument assumes a bounded body and sufficient regularity for [Green's first identity](../../../../green-s-first-identity.md), or the corresponding finite-energy weak formulation.

For the composite body, let $w_-$ and $w_+$ be the differences in $V_1$ and $V_2$. They are [harmonic functions](../../../../harmonic-function.md), have a common interface value $w$, and obey

$$
\alpha\partial_nw_+=\beta\partial_nw_-,\qquad w_+|_{S_2}=0.
$$

The [unit normal vector](../../../../unit-normal.md) $n$ points out of $V_1$; the outward normal of $V_2$ on its inner boundary is $-n$. Keeping that sign in [Green's first identity](../../../../green-s-first-identity.md) gives

$$
E_1:=\int_{V_1}|\nabla w_-|^2dV=\int_{S_1}w\,\partial_nw_-\,dS,
\qquad
E_2:=\int_{V_2}|\nabla w_+|^2dV=-\int_{S_1}w\,\partial_nw_+\,dS.
$$

The outer boundary term in $E_2$ is zero. Weight these equations by the positive coefficients that match the flux condition:

$$
\boxed{\beta E_1+\alpha E_2=\int_{S_1}w\left(\beta\partial_nw_--\alpha\partial_nw_+\right)dS=0.}
$$

Both [Dirichlet energies](../../../../dirichlet-energy.md) must vanish. Hence both differences are constants; the outer data set the constant in $V_2$ to zero, and interface continuity sets the constant in $V_1$ to zero. This establishes [uniqueness for a harmonic transmission problem](../../../../uniqueness-for-a-harmonic-transmission-problem.md). Physically $\beta$ and $\alpha$ play the roles of the inner and outer [thermal conductivities](../../../../thermal-conductivity.md); continuity of temperature and normal heat flux is what cancels the interface contribution.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [Paper 2](../../paper-2-split.md)
3. [2011](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For a [slender viscous thread](../../../../../slender-viscous-thread.md), leading axial velocity is uniform over a section. Incompressibility gives $u_r=-rw_z/2$. The radial and azimuthal strain rates are $-w_z/2$, and the axial one is $w_z$. The [Newtonian fluid stress tensor](../../../../../newtonian-fluid-stress-tensor.md) then has $\sigma_{rr}=-p-\mu w_z$. Matching the inviscid exterior normal stress requires $p=p_a-\mu w_z$, so $\sigma_{zz}=-p_a+3\mu w_z$. The coefficient three is the [Trouton ratio](../../../../../trouton-ratio.md).

A short section has end-stress resultant $\partial_z(A\sigma_{zz})\,dz$. The side's hydrostatic traction adds $p_a A_z\,dz$, and gravity adds $\rho gA\,dz$. Neglecting inertia and capillarity, their sum is zero:

$$
3\mu(Aw_z)_z-A(p_a)_z+\rho gA=0.
$$

Since $(p_a)_z=\rho_a g$, **the balances are**

$$
\boxed{\frac{3\mu}{A}(Aw_z)_z+(\rho-\rho_a)g=0,\qquad
A_t+(Aw)_z=0.}
$$

The second is cross-sectional volume conservation, equivalently $D_tA=-Aw_z$. Small interface slope justifies the sectionwise extensional approximation; the slow-flow assumption is additionally needed to neglect inertia.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 75](../../paper-75-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The logarithmic density term is the [barotropic fluid](../../../../../../barotropic-fluid.md) energy for $p=c_s^2\rho$, rather than the thermodynamic heat content of an isolated gas. Define

$$
e(\rho)=c_s^2\ln(\rho/\rho_0),\qquad
E_h=\rho\left(\frac{v^2}{2}+\Phi+e\right),\qquad
E_B=\frac{B^2}{2\mu_0}.
$$

For any scalar $q$, the [continuity equation](../../../../../../continuity-equation.md) implies $\partial_t(\rho q)+\partial_z(\rho wq)=\rho Dq$. Therefore $De=-c_s^2w'$, $D\Phi=wg$, and dotting the momentum equations with $\rho\mathbf v$ gives

$$
\partial_tE_h+\partial_z(wE_h)
=-\partial_z(wp)
+\frac{B_z}{\mu_0}(v_xB_x'+v_yB_y')
-wE_B'-a\rho v_xv_y.
$$

The [MHD induction equation](../../../../../../ideal-magnetohydrodynamic-induction-equation.md) gives the complementary [magnetic energy](../../../../../../magnetic-energy.md) balance

$$
\partial_tE_B+\partial_z(wE_B)
=\frac{B_z}{\mu_0}(B_xv_x'+B_yv_y')
-\left(E_B-\frac{B_z^2}{\mu_0}\right)w'
+\frac{aB_xB_y}{\mu_0}.
$$

Adding these two identities, and collecting the product derivatives, yields the [barotropic magnetic energy equation](../../../../../../barotropic-magnetic-energy-equation.md)

$$
\boxed{\partial_tE+\partial_zF=S,\qquad
F=w\left(E+p+\frac{B^2}{2\mu_0}\right)
-\frac{B_z}{\mu_0}(\mathbf v\cdot\mathbf B),\qquad
S=a\left(\frac{B_xB_y}{\mu_0}-\rho v_xv_y\right).}
$$

Here $E=E_h+E_B$. The two stress terms in $S$ describe [magnetohydrodynamic shear work](../../../../../../magnetohydrodynamic-shear-work.md): the maintained background [shear flow](../../../../../../shear-flow.md) can supply energy to, or remove energy from, the perturbation flow and [magnetic field](../../../../../../magnetic-field.md). The sign depends on the off-diagonal total stress; this is why the energy excluding the background [shear flow](../../../../../../shear-flow.md) is not generally conserved. Changing $\rho_0$ merely adds a constant multiple of the conserved density to $E$ and the corresponding mass flux to $F$, leaving $S$ unchanged.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 57](../../../paper-57-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

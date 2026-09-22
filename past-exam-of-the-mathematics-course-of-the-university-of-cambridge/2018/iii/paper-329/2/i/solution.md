<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Take $\mathbf F,\mathbf G$ to be the force and couple exerted by the body on the fluid, equivalently the external force and couple needed to maintain its motion. This fixes the sign for a positive [hydrodynamic resistance matrix](../../../../../../hydrodynamic-resistance-matrix.md). If one uses the fluid's force on the body, both resultants have the opposite sign.

For two [Stokes flows](../../../../../../stokes-flow-split.md) $(\mathbf u,\boldsymbol\sigma)$ and $(\widetilde{\mathbf u},\widetilde{\boldsymbol\sigma})$ in the same fluid domain $\mathcal D$, with zero body force, the [Lorentz reciprocal theorem for Stokes flow](../../../../../../lorentz-reciprocal-theorem-for-stokes-flow.md) is

$$
\boxed{\int_{\partial\mathcal D}\mathbf u\cdot\widetilde{\boldsymbol\sigma}\mathbf n\,dS
=\int_{\partial\mathcal D}\widetilde{\mathbf u}\cdot\boldsymbol\sigma\mathbf n\,dS.}
$$

Here $\mathbf n$ points out of the fluid. To see the identity, take the divergence of the difference of the two cross-work fluxes. The stress divergences vanish, while [incompressibility](../../../../../../incompressible-flow.md) and symmetry of the [Newtonian fluid stress tensor](../../../../../../newtonian-fluid-stress-tensor.md) reduce the remaining terms to $2\mu(\mathbf e:\widetilde{\mathbf e}-\widetilde{\mathbf e}:\mathbf e)=0$. The [divergence theorem](../../../../../../divergence-theorem.md) proves the result.

On the body, the [no-slip boundary condition](../../../../../../no-slip-boundary-condition.md) is $\mathbf u=\mathbf U+\boldsymbol\Omega\times\mathbf r$, and the far-field contribution vanishes for decaying exterior flows. Reciprocity becomes

$$
\mathbf U\cdot\widetilde{\mathbf F}+\boldsymbol\Omega\cdot\widetilde{\mathbf G}
=\widetilde{\mathbf U}\cdot\mathbf F+\widetilde{\boldsymbol\Omega}\cdot\mathbf G.
$$

With $q=(\mathbf U,\boldsymbol\Omega)^T$ and $(\mathbf F,\mathbf G)^T=\mathsf Rq$, this is $q^T\mathsf R\widetilde q=\widetilde q^T\mathsf Rq$ for all pairs, so $\mathsf R^T=\mathsf R$. The power identity gives

$$
q^T\mathsf Rq=\mathbf F\cdot\mathbf U+\mathbf G\cdot\boldsymbol\Omega
=2\mu\int_{\mathcal D}\mathbf e:\mathbf e\,dV\ge0.
$$

Equality would force zero strain throughout the connected exterior domain, hence a rigid fluid motion. Decay at infinity makes that motion zero, and the [no-slip boundary condition](../../../../../../no-slip-boundary-condition.md) then gives $q=0$. This proves the [symmetry and positivity of a rigid-body resistance matrix](../../../../../../symmetry-and-positivity-of-a-rigid-body-resistance-matrix.md):

$$
\boxed{\mathsf R^T=\mathsf R,\qquad q^T\mathsf Rq>0\text{ for }q\ne0.}
$$

For the [helix](../../../../../../helix.md), assume $0<\phi<\pi/2$ and use cylindrical unit vectors. Its arclength element and tangent are

$$
\frac{ds}{d\theta}=\left|\frac{d\mathbf X}{d\theta}\right|=b\sec\phi,
\qquad\mathbf t=\frac{d\mathbf X}{ds}=\cos\phi\,\mathbf e_\theta+\sin\phi\,\mathbf e_z.
$$

Integrating to $\theta=L\cos\phi/b$ gives $\boxed{\text{total arc length}=L}$. In a combined axial translation and rotation, $\mathbf V=U\mathbf e_z+b\Omega\mathbf e_\theta$. The [slender-body force density](../../../../../../slender-body-force-density.md), or local [resistive-force theory](../../../../../../resistive-force-theory.md), gives

$$
\mathbf f=C\left[\mathbf V-\frac12\mathbf t(\mathbf t\cdot\mathbf V)\right],
\qquad C=\frac{4\pi\mu}{|\log\epsilon|}.
$$

Writing $s_\phi=\sin\phi$, $c_\phi=\cos\phi$, its axial and azimuthal components are

$$
f_z=C\left[(1-s_\phi^2/2)U-bs_\phi c_\phi\Omega/2\right],\qquad
f_\theta=C\left[b(1-c_\phi^2/2)\Omega-s_\phi c_\phi U/2\right].
$$

The axial couple density is $bf_\theta$. Integration over arclength gives the [axial resistance matrix of a slender helix](../../../../../../axial-resistance-matrix-of-a-slender-helix.md):

$$
\boxed{\begin{pmatrix}F_z\\G_z\end{pmatrix}
=\begin{pmatrix}A&B\\B&D\end{pmatrix}\begin{pmatrix}U\\\Omega\end{pmatrix},\quad
A=\frac{CL}{2}(1+c_\phi^2),\quad
B=-\frac{CLb}{2}s_\phi c_\phi,\quad
D=\frac{CLb^2}{2}(1+s_\phi^2).}
$$

Thus pure translation gives $(F_z,G_z)=(AU,BU)$, and pure rotation gives $(F_z,G_z)=(B\Omega,D\Omega)$. The mixed coefficients agree, as reciprocity requires, and $AD-B^2=C^2L^2b^2/2>0$. The sign of $B$ follows the handedness in the parametrization; reversing handedness reverses propulsion.

For the [helical microswimmer with a spherical head](../../../../../../helical-microswimmer-with-a-spherical-head.md), the diagram's rotation relation is $\Omega_0=\Omega-\omega$. Neutral buoyancy and the absence of external forcing make the whole swimmer [force-free](../../../../../../force-free.md) and [torque-free](../../../../../../torque-free.md). Neglecting interactions between its parts gives

$$
(A_0+A)U+B\Omega=0,\qquad
BU+D\Omega+D_0(\Omega-\omega)=0.
$$

With $\Delta=(A_0+A)(D_0+D)-B^2>0$, solving this pair gives

$$
\boxed{U=-\frac{BD_0\omega}{\Delta},\qquad
\Omega=\frac{(A_0+A)D_0\omega}{\Delta},\qquad
\Omega_0=-\frac{(A_0+A)D-B^2}{\Delta}\omega.}
$$

The head counterrotates, providing the reaction to the flagellum's rotation. The figure fixes this relative rotation convention; it is duplicated and corrupted in the local TeX.

For a very large head, the coefficient regime is $A_0\gg A$ and $D_0\gg D$. Consequently

$$
\boxed{U\simeq-\frac{B\omega}{A_0},\qquad\Omega\simeq\omega\quad(a\gg L).}
$$

The large translational resistance $A_0$ makes the [microswimmer](../../../../../../microswimmer.md) slow even though the flagellum rotates almost at the motor rate.

For a very small head, $A_0\ll A$ and $D_0\ll D$. The appropriate denominator retains the translation-rotation coupling:

$$
\boxed{U\simeq-\frac{BD_0\omega}{AD-B^2},\qquad
\Omega\simeq\frac{AD_0\omega}{AD-B^2}\quad(a\ll(Lb^2)^{1/3}).}
$$

Both tend to zero with $D_0\propto a^3$, while $\Omega_0\simeq-\omega$. The motor mainly rotates the low-resistance head, and produces little flagellar motion relative to the fluid.

In the intermediate coefficient regime $A_0\ll A$ and $D_0\gg D$, the head supplies a strong rotational reaction with little translational penalty. Then

$$
\boxed{U\simeq-\frac{B\omega}{A}
=\omega b\frac{\sin\phi\cos\phi}{1+\cos^2\phi},\qquad\Omega\simeq\omega.}
$$

The head radius has dropped out. To find the [optimal pitch of a helical microswimmer](../../../../../../optimal-pitch-of-a-helical-microswimmer.md), put $z=\tan\phi$. The dimensionless speed becomes $z/(z^2+2)$ and has derivative $(2-z^2)/(z^2+2)^2$. Hence, for $\omega>0$ with the chosen handedness,

$$
\boxed{\tan\phi_{\mathrm{opt}}=\sqrt2,\qquad
\phi_{\mathrm{opt}}\simeq54.74^\circ,\qquad U_{\max}=\frac{\omega b}{2\sqrt2}.}
$$

The angle is measured from the horizontal plane. An intermediate pitch combines axial and transverse tangent directions, allowing anisotropic drag to convert rotation into translation; either extreme removes that coupling.

The geometric head-size regimes quoted in the paper hold with the logarithmic slenderness factor treated as fixed. More precisely, $A_0\ll A$ requires $a\ll L(1+\cos^2\phi)/(3|\log\epsilon|)$, while $D_0\gg D$ requires $a^3\gg Lb^2(1+\sin^2\phi)/(4|\log\epsilon|)$. These coefficient inequalities state the validity of the intermediate approximation when the logarithm is quantitatively important. The many-turn and local-drag assumptions of [slender-body theory](../../../../../../slender-body-theory.md) also remain in force.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 329](../../../paper-329-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

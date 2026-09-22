<h1 id="h2/solution">Solution</h1>

↑ **Parent:** [H2](../h2.md)

Differentiating orthonormality gives $\dot e_i\cdot e_j=-e_i\cdot\dot e_j$. With $\omega=\tfrac12\sum_i e_i\times\dot e_i$, the [vector](../../../vector.md) triple product yields

$$
\omega\times e_j=\tfrac12\left(\dot e_j-\sum_i e_i(\dot e_i\cdot e_j)\right)=\dot e_j.
$$

The body coordinates $x_i$ of a fixed material point are constant. Differentiating its position $R_G+\sum_ix_ie_i$ therefore gives

$$
\boxed{v=v_G+\omega\times r.}
$$

This identifies $\omega$ as the [angular velocity](../../../angular-velocity.md) of the [rigid body](../../../rigid-body-dynamics-split.md).

Because $G$ is the [center of mass](../../../center-of-mass.md), $\int\rho r\,dV=0$, so the translational contribution to the [angular momentum](../../../angular-momentum.md) about $G$ vanishes. The remaining [vector](../../../vector.md) triple product gives

$$
L=\int\rho\{(r\cdot r)\omega-(r\cdot\omega)r\}\,dV,
\qquad
\boxed{J_{ij}=\int\rho\left(|r|^2\delta_{ij}-x_ix_j\right)dV,\quad L_i=\sum_jJ_{ij}\omega_j.}
$$

This symmetric [matrix](../../../matrix.md) is the [inertia tensor](../../../inertia-tensor.md) about $G$. The angular-momentum balance about the center of mass is $dL/dt=\tau_{\mathrm{ext},G}$ in an inertial frame. With no external forces, that torque is zero, so **the inertial [vector](../../../vector.md) $L$ is constant**. Its components in rotating body axes need not individually be constant.

For the tool, let the disc lie at $z=0$ and the rod extend to $z=l=\sqrt3a$. The total mass is $3M$ and its center is at $z_G=l/3$. Axial symmetry makes the [inertia tensor](../../../inertia-tensor.md) diagonal with $I_x=I_y$.

The standard disc moments are $MR^2/2$ about its normal and $MR^2/4$ about a diameter. A thin rod has moment $ml^2/12$ about a transverse axis through its center. The [parallel axis theorem](../../../parallel-axis-theorem.md) adds $md^2$ for a parallel shift of distance $d$. Therefore

$$
I_z=\tfrac12M(2a)^2=2Ma^2,
$$

and

$$
\begin{aligned}
I_x=I_y
&=Ma^2+M(l/3)^2+\frac{2Ml^2}{12}+2M(l/6)^2\\
&=Ma^2+\frac{Ml^2}{3}=2Ma^2.
\end{aligned}
$$

The rod contributes zero about its own longitudinal axis. Thus $\boxed{J=2Ma^2I_3}$, an isotropic [inertia tensor](../../../inertia-tensor.md) even though the shape is not spherical. This gives a [nonspherical rigid body with isotropic inertia](../../../nonspherical-rigid-body-with-isotropic-inertia.md). Consequently $L=2Ma^2\omega$. Conservation of $L$ in torque-free motion proves **the [angular velocity](../../../angular-velocity.md) is constant for every initial orientation and spin**.

## ↑ Ancestors (11)

1. [H2](../h2.md)
2. [2013](../../2013-split.md)
3. [Past exam of the options II course of the University of Oxford](../../split.md)
4. [Options II course of the University of Oxford](../../../options-ii-course-of-the-university-of-oxford.md)
5. [Year 2 of the mathematics course of the University of Oxford](../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)

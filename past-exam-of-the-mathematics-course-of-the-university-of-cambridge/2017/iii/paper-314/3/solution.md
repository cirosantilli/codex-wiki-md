<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Write $c_s^2=p/\rho$ for the constant [isothermal sound speed](../../../../../isothermal-sound-speed.md) squared and $v_a^2=B^2/(\mu_0\rho)$ for the constant [Alfvén speed](../../../../../alfven-speed.md) squared. The horizontal [magnetic field](../../../../../magnetic-field.md) has no vertical [magnetic tension](../../../../../magnetic-tension.md); [magnetostatic equilibrium](../../../../../magnetostatic-equilibrium.md) is

$$
\frac{d\Pi}{dz}=-g\rho,\qquad \Pi=p+\frac{B^2}{2\mu_0}=\left(c_s^2+\frac{v_a^2}{2}\right)\rho.
$$

Consequently the [magnetized isothermal atmosphere](../../../../../magnetized-isothermal-atmosphere.md) has

$$
\boxed{H=\frac{c_s^2+v_a^2/2}{g},\qquad
\rho=\rho_0e^{-z/H},\qquad p=c_s^2\rho_0e^{-z/H},\qquad
B=B_0e^{-z/(2H)},\quad B_0^2=\mu_0\rho_0v_a^2.}
$$

The sign of $B_0$ specifies the orientation of the [magnetic field](../../../../../magnetic-field.md). The [adiabatic sound speed](../../../../../adiabatic-sound-speed.md) is $v_s^2=\gamma p/\rho=\gamma c_s^2$, also constant.

For the proposed [normal mode](../../../../../normal-mode.md), let $A=\exp(i\mathbf k\cdot\mathbf x+z/(2H)-i\omega t)$, $a=1/(2H)$, and temporarily write $\boldsymbol\xi$ for its constant complex amplitude. The [divergence](../../../../../divergence.md) amplitude is $\Delta=ik_x\xi_x+ik_y\xi_y+(ik_z+a)\xi_z$. Using $\rho'/\rho=-1/H$ and $B'/B=-a$, the [Eulerian and Lagrangian fluid perturbations](../../../../../eulerian-and-lagrangian-fluid-perturbations.md) give

$$
\frac{\delta\rho}{\rho A}=-\Delta+\frac{\xi_z}{H},\qquad
\frac{\delta\mathbf B}{BA}=ik_y\boldsymbol\xi-\mathbf e_y\Delta+a\mathbf e_y\xi_z.
$$

Since $\Pi'/\rho=-g$, the [magnetohydrodynamic total pressure](../../../../../magnetohydrodynamic-total-pressure.md) amplitude is

$$
\psi=\frac{\delta\Pi}{\rho A}=-(v_s^2+v_a^2)\Delta+v_a^2ik_y\xi_y+g\xi_z.
$$

The vertical derivative of $\delta\Pi=\rho A\psi$ is $\rho A(ik_z-a)\psi$. For the [magnetic tension](../../../../../magnetic-tension.md) perturbation, the terms proportional to $aik_y\xi_z\mathbf e_y$ from $\delta\mathbf B\cdot\nabla\mathbf B$ and $\mathbf B\cdot\nabla\delta\mathbf B$ cancel, leaving

$$
\frac{\delta\mathbf B\cdot\nabla\mathbf B+\mathbf B\cdot\nabla\delta\mathbf B}{\mu_0\rho A}
=-v_a^2 k_y^2\boldsymbol\xi-v_a^2ik_y\Delta\,\mathbf e_y.
$$

Thus the [linearization](../../../../../linearization.md) really reduces to the constant-coefficient [eigenvalue problem](../../../../../eigenvalue-problem.md)

$$
\begin{aligned}
-\omega^2\xi_x&=-ik_x\psi-k_y^2v_a^2\xi_x,\\
-\omega^2\xi_y&=-ik_y(\psi+v_a^2\Delta)-k_y^2v_a^2\xi_y,\\
-\omega^2\xi_z&=g(\Delta-\xi_z/H)-(ik_z-a)\psi-k_y^2v_a^2\xi_z.
\end{aligned}
$$

For a static [ideal magnetohydrodynamics](../../../../../ideal-magnetohydrodynamics.md) equilibrium with conservative [gravitational acceleration](../../../../../gravitational-acceleration.md), the [magnetohydrodynamic energy principle](../../../../../magnetohydrodynamic-energy-principle.md) gives a [Hermitian operator](../../../../../hermitian-operator.md) for the restoring force in the [mass density](../../../../../density.md) weighted [inner product](../../../../../inner-product.md), provided the surface terms vanish. The factor $e^{z/(2H)}$ removes the exponential [mass density](../../../../../density.md) weight. This can be checked directly, without assuming stability: set $s=v_s^2$, $b=v_a^2$, and $q=s+b$. Then $\omega^2\boldsymbol\xi=\mathsf K\boldsymbol\xi$, where

$$
\mathsf K=
\begin{pmatrix}
qk_x^2+bk_y^2&sk_xk_y&qk_xk_z+ik_x(g-qa)\\
sk_xk_y&sk_y^2&sk_yk_z+ik_y(g-sa)\\
qk_xk_z-ik_x(g-qa)&sk_yk_z-ik_y(g-sa)&q(k_z^2+a^2)+bk_y^2
\end{pmatrix}.
$$

This is a [Hermitian matrix](../../../../../hermitian-operator.md) for real $\mathbf k$ and real positive $s,b$. Therefore **every squared frequency $\omega^2$ is real**; negative values give exponential growth, rather than an oscillation with a complex squared frequency. In an infinite atmosphere these are generalized [plane waves](../../../../../plane-wave.md), not finite-total-energy global modes.

At $\omega^2=0$ and $k_y\ne0$, the $y$ equation, after cancelling its magnetic terms, gives $s\Delta=g\xi_z$. For nonzero [magnetic field](../../../../../magnetic-field.md), the $x$ equation also gives $ik_x\xi_x=k_x^2\psi/(k_y^2b)$. Substituting $\psi=-b[\Delta-ik_y\xi_y]+g\xi_z-s\Delta$ and then $s\Delta=g\xi_z$ yields

$$
\boxed{s\Delta=g\xi_z,\qquad -(k_x^2+k_y^2)\psi=k_y^2b(ik_z+a)\xi_z.}
$$

For a nontrivial mode $\xi_z\ne0$; otherwise these equations and $k_yb\ne0$ force every component to vanish. Substitution in the vertical equation gives

$$
\boxed{b k_y^2\left(|\mathbf k|^2+\frac{1}{4H^2}\right)+\frac gH\left(1-\frac{gH}{s}\right)(k_x^2+k_y^2)=0.}
$$

For example, the [determinant](../../../../../determinant.md) provides an independent check:

$$
\det\mathsf K=s b k_y^2\left[b k_y^2(|\mathbf k|^2+a^2)+\left(\frac gH-\frac{g^2}{s}\right)(k_x^2+k_y^2)\right].
$$

To prove the claimed “if and only if”, rather than merely locating a zero [eigenvalue](../../../../../eigenvalue.md), use the [magnetic buoyancy energy criterion](../../../../../magnetic-buoyancy-energy-criterion.md)

$$
\begin{aligned}
\boldsymbol\xi^\dagger\mathsf K\boldsymbol\xi={}&s\left|\Delta-\frac g{s}\xi_z\right|^2
+b\left|ik_x\xi_x+(ik_z+a)\xi_z\right|^2\\
&+bk_y^2(|\xi_x|^2+|\xi_z|^2)
+\left(\frac gH-\frac{g^2}{s}\right)|\xi_z|^2.
\end{aligned}
$$

If $gH\leq s$, every term is nonnegative, so all [eigenvalues](../../../../../eigenvalue.md) are nonnegative for every [wavevector](../../../../../wavevector.md), including $k_y=0$. If $gH>s$, choose $k_z=0$, any fixed $k_x\ne0$, and $\xi_z=1$, $\xi_x=-a/(ik_x)$, $\xi_y=g/(sik_y)$. The first two squares vanish; the remaining value is

$$
bk_y^2\left(1+\frac{a^2}{k_x^2}\right)+\frac gH-\frac{g^2}{s},
$$

which is negative for sufficiently small nonzero $k_y$. The [Rayleigh quotient](../../../../../rayleigh-quotient.md) of this displacement is therefore negative, proving a negative [eigenvalue](../../../../../eigenvalue.md) and an unstable [normal mode](../../../../../normal-mode.md). This uses precisely the assumption that [boundary conditions](../../../../../boundary-condition.md) do not exclude the chosen wavelengths. Equality is a neutral threshold, not exponential growth.

Finally the [plasma beta](../../../../../plasma-beta.md) is $\beta=p/[B^2/(2\mu_0)]=2c_s^2/v_a^2$. Hence

$$
\boxed{\text{instability}\ \Longleftrightarrow\ gH>v_s^2
\ \Longleftrightarrow\ \frac{v_a^2}{2}>(\gamma-1)c_s^2
\ \Longleftrightarrow\ \beta(\gamma-1)<1.}
$$

The [magnetic field](../../../../../magnetic-field.md) is assumed nonzero in the marginal-mode elimination and in the finite $\beta$ expression. The positive-sound-speed, nonmagnetic limit remains covered by the energy identity; for the usual $\gamma>1$ it is stable. [Parker instability](../../../../../parker-instability.md) occurs because [magnetic pressure](../../../../../magnetic-pressure.md) supports part of the atmosphere's weight while the gas can drain along gently bent [magnetic field lines](../../../../../magnetic-field-line.md). The resulting buoyant displacement can release [Newtonian gravitational potential energy](../../../../../newtonian-gravitational-potential-energy.md); choosing long wavelengths along the [magnetic field](../../../../../magnetic-field.md) makes the stabilizing [magnetic tension](../../../../../magnetic-tension.md) small. The completed-square calculation quantifies this competition, including the [adiabatic process](../../../../../adiabatic-process.md) restoring force.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 314](../../paper-314-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Reflection in $y=0$ preserves the prescribed translational [velocity](../../../../../velocity.md) and axial [angular velocity](../../../../../angular-velocity.md). A [force](../../../../../force.md) transforms as a polar [vector](../../../../../vector.md), whereas a [torque](../../../../../torque.md) transforms as an axial vector; consequently $F_y=G_x=G_z=0$. Reflection in $x=0$ reverses both imposed motions but preserves the normal force component. The [linearity](../../../../../linearity.md) of [Stokes flow](../../../../../stokes-flow-split.md) then gives $F_z=0$. Thus only $F_x$ and $G_y$ can be nonzero.

There is a sign inconsistency in the printed question. In right-handed coordinates, $\boldsymbol\Omega=\Omega\mathbf e_y$ gives a rotational velocity $-\Omega a\mathbf e_x$ at the sphere's lowest point. The printed shear and force formulas instead use the opposite rotational sense. Below, let $\omega$ be the right-handed component along $+\mathbf e_y$; the paper's displayed formulas are recovered by setting $\omega=-\Omega$.

In the translating frame, the parabolic gap and leading boundary velocities are

$$
h=a\epsilon+\frac{x^2+y^2}{2a},\qquad
\mathbf v_\parallel(0)=-U\mathbf e_x,\qquad
\mathbf v_\parallel(h)=-\omega a\mathbf e_x.
$$

The [no-slip boundary condition](../../../../../no-slip-boundary-condition.md) and [lubrication theory](../../../../../lubrication-theory.md) give

$$
\mathbf v_\parallel(z)=\frac{z(z-h)}{2\mu}\nabla_\parallel p-U\mathbf e_x+(U-\omega a)\frac zh\mathbf e_x,
\qquad
\mathbf q=-\frac{h^3}{12\mu}\nabla_\parallel p-\frac h2(U+\omega a)\mathbf e_x.
$$

The gap is stationary in this frame, so $\nabla_\parallel\cdot\mathbf q=0$. The [Reynolds lubrication equation](../../../../../reynolds-equation.md) is therefore

$$
\nabla_\parallel\cdot(h^3\nabla_\parallel p)=-6\mu(U+\omega a)h_x.
$$

Since $h_x=x/a$ and $\nabla_\parallel^2h=2/a$,

$$
\nabla_\parallel\cdot\left[h^3\nabla_\parallel(x/h^2)\right]=-5x/a,
\qquad
\boxed{p=\frac{6\mu}{5}(U+\omega a)\frac{x}{h^2}.}
$$

Differentiating the velocity profile gives the leading [shear stresses](../../../../../shear-stress.md)

$$
\begin{aligned}
\frac{\sigma_{xz}(0)}\mu&=\frac{6(U+\omega a)x^2}{5ah^2}+\frac{2U-8\omega a}{5h},\\
\frac{\sigma_{xz}(h)}\mu&=-\frac{6(U+\omega a)x^2}{5ah^2}+\frac{8U-2\omega a}{5h},\\
\frac{\sigma_{yz}(0)}\mu&=\frac{6(U+\omega a)xy}{5ah^2},\\
\frac{\sigma_{yz}(h)}\mu&=-\frac{6(U+\omega a)xy}{5ah^2}.
\end{aligned}
$$

The first expression becomes the printed formula after $\omega=-\Omega$.

For the [logarithmic lubrication resistance of a sphere near a wall](../../../../../logarithmic-lubrication-resistance-of-a-sphere-near-a-wall.md), write $\ell=\log(1/\epsilon)$. The logarithmic region is $a\sqrt\epsilon\ll r\ll a$, where $h\sim r^2/(2a)$. Consequently

$$
\int\frac{dx\,dy}{h}=2\pi a\ell+O(a),\qquad
\int\frac{x^2\,dx\,dy}{ah^2}=2\pi a\ell+O(a).
$$

These follow from $\int r/h\,dr=a\ell+O(a)$ and $\int r^3/h^2\,dr=2a^2\ell+O(a^2)$, with a fixed small outer cutoff. The general logarithmic radial numerator is $r^{2n-1}$ over $h^n$; the numerator in the printed integration hint appears to have a typographical error.

The force exerted on the fluid through the upper gap boundary includes pressure acting on its slope:

$$
F_x=\int\left[\sigma_{xz}(h)+p h_x\right]dx\,dy.
$$

The pressure cancels the $x^2/h^2$ term, giving

$$
\boxed{F_x=\frac{4\pi\mu a}{5}(4U-\omega a)\ell+O\!\left(\mu a(|U|+a|\omega|)\right).}
$$

Pressure exerts no [torque](../../../../../torque.md) about the centre of a sphere because its traction is radial. To logarithmic order, the shear has lever arm $-a\mathbf e_z$, so

$$
G_y=-a\int\sigma_{xz}(h)dx\,dy
=\frac{4\pi\mu a^2}{5}(4\omega a-U)\ell+O\!\left(\mu a^2(|U|+a|\omega|)\right).
$$

The other components vanish by parity: $G_x$ involves an integral of the $xy$ term, and $G_z$ has an integrand odd in $y$. The combined [hydrodynamic resistance matrix](../../../../../hydrodynamic-resistance-matrix.md) is

$$
\boxed{\begin{pmatrix}F_x\\G_y/a\end{pmatrix}\sim\frac{4\pi\mu a}{5}\ell\begin{pmatrix}4&-1\\-1&4\end{pmatrix}\begin{pmatrix}U\\a\omega\end{pmatrix}.}
$$

Its equal off-diagonal coefficients are required by the [Lorentz reciprocal theorem for Stokes flow](../../../../../lorentz-reciprocal-theorem-for-stokes-flow.md). It is a [positive-definite matrix](../../../../../positive-definite-matrix.md), as required by [viscous dissipation](../../../../../viscous-dissipation.md).

In the rotational convention of the printed force formula, set $\Omega=-\omega$ and measure the scalar couple along $-\mathbf e_y$, so $G=-G_y$. Then

$$
\boxed{F\sim\frac{4\pi\mu a}{5}(4U+a\Omega)\ell,\qquad
G\sim\frac{4\pi\mu a^2}{5}(U+4a\Omega)\ell.}
$$

For sedimentation under the buoyancy-adjusted weight $F$, a uniform sphere is [torque-free](../../../../../torque-free.md). Thus $\omega a=U/4$, and the force balance gives

$$
\boxed{U\sim\frac{F}{3\pi\mu a\log(1/\epsilon)},\qquad
\omega\sim\frac{F}{12\pi\mu a^2\log(1/\epsilon)}.}
$$

The rotational scalar in the paper's displayed-force convention is $\Omega=-U/(4a)$. The sphere rolls in the right-handed $+\mathbf e_y$ sense but still slips: its lowest point has laboratory velocity $U-a\omega=3U/4$. The signs and coefficients of the right-handed resistance agree with the rigid-wall terms of [Bertin et al., equations (4.4)–(4.5)](https://vincent-bertin.github.io/Papers/09_Bertin2022JFM.pdf), after reversing the forces and torques there from fluid-on-sphere to sphere-on-fluid.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 329](../../paper-329-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

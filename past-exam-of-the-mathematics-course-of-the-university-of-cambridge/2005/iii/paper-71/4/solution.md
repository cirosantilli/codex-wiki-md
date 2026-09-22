<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Set $a=2\pi G\rho_0$. The axisymmetric [Poisson equation for Newtonian gravity](../../../../../poisson-equation-for-newtonian-gravity.md) integrates to $(R\Phi_R)'=4\pi G\rho_0R$. Regularity on the axis fixes the integration constant, so $\Phi_R=aR$. Radial force balance in the [rotating fluid](../../../../../rotating-fluid.md) gives

$$
p_R=\rho_0(R\Omega^2-\Phi_R)=\rho_0(k^2R^3-aR),\qquad
p=p_c+\rho_0\left(\frac{k^2R^4}{4}-\frac{aR^2}{2}\right).
$$

With the stated central [pressure](../../../../../pressure.md), $p_c=\rho_0a^2/(4k^2)$, this is a perfect square:

$$
\boxed{p(R)=\frac{\rho_0k^2}{4}(R^2-R_0^2)^2,\qquad R_0^2=\frac{a}{k^2}=\frac{2\pi G\rho_0}{k^2}.}
$$

The [free surface](../../../../../free-surface.md) lies at the first zero of [pressure](../../../../../pressure.md). For the source's positive rotation parameter, $R_0=\sqrt{2\pi G\rho_0}/k$; allowing either rotation direction requires $|k|$ in the denominator. The inward effective gravity is $\Phi_R-R\Omega^2=R(a-k^2R^2)$, so **$\boxed{g_{\rm eff}(R_0)=0}$**. In particular $p_R(R_0)=0$. This is the [critically rotating self-gravitating cylinder](../../../../../critically-rotating-self-gravitating-cylinder.md).

For a [normal mode](../../../../../normal-mode.md) proportional to $e^{i\omega t+im\phi}$, the background [material derivative](../../../../../material-derivative.md) becomes $i\sigma$, where $\sigma=\omega+m\Omega(R)$. Linearizing the centrifugal term gives $-2\Omega u_\phi$ in the radial equation. In the azimuthal equation the background [velocity](../../../../../velocity.md) gradient and cylindrical geometric term together give $(2\Omega+R\Omega')u_R=3\Omega u_R$. Since the interior [mass density](../../../../../density.md) is constant, write $W=p'/\rho_0+\Phi'$. The two momentum equations and [incompressible flow](../../../../../incompressible-flow.md) condition are consequently

$$
\boxed{\begin{aligned}
i\sigma u_R-2\Omega u_\phi&=-W',\\
3\Omega u_R+i\sigma u_\phi&=-imW/R,\\
u_R'+u_R/R+im u_\phi/R&=0.
\end{aligned}}
$$

For $m\ne0$, the last two equations express the other amplitudes in terms of $u=u_R$:

$$
u_\phi=\frac{i}{m}(Ru'+u),\qquad W=\frac{iR}{m^2}\{3m\Omega u-\sigma(Ru'+u)\}.
$$

Differentiate the second expression using $R\Omega'=\Omega$ and $R\sigma'=m\Omega$, then substitute into the radial momentum equation. Before any division by $\sigma$, the result is

$$
-\sigma R^2u''-3\sigma Ru'+[3m\Omega+(m^2-1)\sigma]u=0.
$$

Away from corotation this gives the required [ordinary differential equation](../../../../../ordinary-differential-equation.md)

$$
\boxed{u''+\frac3R u'+\frac{u}{R^2}\left(1-m^2-\frac{3m\Omega}{\sigma}\right)=0.}
$$

At corotation the original coupled equations, or the undivided equation, must be used. A regular axisymmetric radial [velocity](../../../../../velocity.md) would vanish by the [incompressible flow](../../../../../incompressible-flow.md) condition; the requested dipolar calculation has $m=1$.

For $m=1$, use the amplitude normalization $u=A(\omega+kR)$, which remains useful when $\omega$ tends to zero. Substitution into the undivided equation gives zero identically. For nonzero $\omega$ this is the source's $1+kR/\omega$ after choosing $A=1/\omega$. The other amplitudes are

$$
\boxed{u_R=A(\omega+kR),\qquad u_\phi=iA(\omega+2kR),\qquad W=iAR[(kR)^2-\omega^2].}
$$

These formulas also satisfy the three original equations directly. By the regularity assumption in the question, this is the interior [velocity](../../../../../velocity.md) family to which the [free surface](../../../../../free-surface.md) conditions must be applied.

The [gravitational potential of a displaced cylindrical interface](../../../../../gravitational-potential-of-a-displaced-cylindrical-interface.md) supplies an essential part of those conditions. For surface [fluid displacement](../../../../../lagrangian-displacement-fluid-mechanics.md) $\eta e^{im\phi}$, the bulk [mass density](../../../../../density.md) perturbation vanishes but the displaced [mass density](../../../../../density.md) step contributes $\rho_0\eta\delta(R-R_0)$. The interior and exterior [gravitational potential](../../../../../newtonian-potential-of-a-point-mass.md) amplitudes solve [Laplace's equation](../../../../../laplace-equation.md), are proportional to $R^m$ and $R^{-m}$ for $m\geq1$, and are continuous at the surface. Integrating the [Poisson equation for Newtonian gravity](../../../../../poisson-equation-for-newtonian-gravity.md) across the [mass density](../../../../../density.md) step gives

$$
\Phi'_{R,\mathrm{out}}-\Phi'_{R,\mathrm{in}}=4\pi G\rho_0\eta.
$$

Since the two radial derivatives at the surface are $-m\Phi'_s/R_0$ and $m\Phi'_s/R_0$, respectively,

$$
\boxed{\Phi'_s=-\frac{aR_0}{m}\eta.}
$$

It would be incorrect to set the entire potential perturbation to zero merely because the bulk [mass density](../../../../../density.md) is unchanged.

Let $\Omega_s=kR_0$, so $a=\Omega_s^2$. Zero [fluid Lagrangian perturbation](../../../../../lagrangian-perturbation-of-a-fluid-variable.md) of surface [pressure](../../../../../pressure.md) gives $p'_s+\eta p_R(R_0)=0$, hence $p'_s=0$. The surface momentum potential and kinematic condition for $m=1$ are therefore

$$
W_s=-\Omega_s^2R_0\eta,\qquad i(\omega+\Omega_s)\eta=A(\omega+\Omega_s).
$$

If $\omega+\Omega_s\ne0$, the kinematic condition fixes $\eta=-iA$. The same value follows if the radial [fluid Lagrangian displacement](../../../../../lagrangian-displacement-fluid-mechanics.md) $u_R/[i(\omega+kR)]=-iA$ is required to extend continuously to the [free surface](../../../../../free-surface.md), including a possible surface-corotation limit. Comparing the gravitational condition with the interior value of $W_s$ then gives

$$
iAR_0(\Omega_s^2-\omega^2)=iAR_0\Omega_s^2,\qquad \boxed{\omega^2=0}
$$

for a nontrivial perturbation. These [dipolar perturbations of a critically rotating cylinder](../../../../../dipolar-perturbations-of-a-critically-rotating-cylinder.md) describe a displacement of the whole cylinder's axis. Translating an isolated self-gravitating system gives another equilibrium, so there is no external restoring force and the translation is neutral. A uniform drift of the centre also follows from invariance under a [Galilean transformation](../../../../../galilean-transformation.md), explaining the double zero of the frequency equation. The singular $1/\omega$ in the originally chosen [velocity](../../../../../velocity.md) normalization does not obstruct the finite-amplitude limiting solution.

There is an admissibility qualification to the frequency conclusion as printed. Regular interior [fluid Eulerian perturbation](../../../../../eulerian-perturbation-of-a-fluid-variable.md) of [velocity](../../../../../velocity.md) alone does not justify cancelling the surface factor $\omega+\Omega_s$. Eliminating $\eta$ without that cancellation instead gives

$$
A\omega^2(\omega+\Omega_s)=0.
$$

The additional surface-corotation case $\omega=-\Omega_s$ formally satisfies every displayed [velocity](../../../../../velocity.md) equation and the usual linearized surface conditions with

$$
\eta=0,\qquad \Phi'=0,\qquad u_R=A(kR-\Omega_s),\qquad
u_\phi=iA(2kR-\Omega_s),\qquad p'=\rho_0iAR[(kR)^2-\Omega_s^2].
$$

Here $u_R(R_0)=p'(R_0)=0$, and the [velocity](../../../../../velocity.md) is finite on the axis. However, its interior radial [fluid Lagrangian displacement](../../../../../lagrangian-displacement-fluid-mechanics.md) tends to $-iA$, whereas the undisplaced surface has $\eta=0$. Thus a regular single-frequency [fluid Lagrangian displacement](../../../../../lagrangian-displacement-fluid-mechanics.md) continuous up to the surface excludes this degenerate branch. **The intended $\omega^2=0$ conclusion holds with that regular-displacement condition, or with surface corotation excluded; the printed [velocity](../../../../../velocity.md) regularity assumption by itself leaves this formal exception.**

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 71](../../paper-71-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

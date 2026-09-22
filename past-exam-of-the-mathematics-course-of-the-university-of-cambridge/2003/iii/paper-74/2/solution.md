<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Write the perturbation [Stokes streamfunction](../../../../../stokes-streamfunction.md) as $\psi=\phi(r)e^{ikz-i\omega t}$, with $\omega=kc$ and nonzero $k$. Its radial and axial [velocity](../../../../../velocity.md) [amplitudes](../../../../../wave-amplitude.md) are $u=-ik\phi/r$ and $w=\phi'/r$. These automatically obey [incompressibility](../../../../../incompressible-flow.md). Linearizing the radial and axial [Euler equations](../../../../../euler-equations-for-an-inviscid-fluid.md), with [pressure](../../../../../pressure.md) [amplitude](../../../../../wave-amplitude.md) $P$, gives

$$
ik(U-c)u=-P'/\rho_0,\qquad ik(U-c)w+U'u=-ikP/\rho_0.
$$

Thus

$$
P/\rho_0=-(U-c)\phi'/r+U'\phi/r,\qquad P'/\rho_0=-k^2(U-c)\phi/r.
$$

Differentiating the first expression, the terms involving $U'\phi'$ cancel. Equating the two expressions for $P'$ proves the [axisymmetric inviscid pipe stability equation](../../../../../axisymmetric-inviscid-pipe-stability-equation.md):

$$
\boxed{(U-c)\left[r\left(\frac{\phi'}r\right)'-k^2\phi\right]-r\left(\frac{U'}r\right)'\phi=0}.
$$

At the axis, finite smooth axisymmetric [velocity](../../../../../velocity.md) requires $\phi=O(r^2)$, after choosing the irrelevant constant in the [streamfunction](../../../../../stream-function.md). At the wall, impermeability gives $\phi(a)=0$. There is no tangential no-slip condition in this inviscid problem. A decoupled azimuthal disturbance satisfies $ik(U-c)u_\theta=0$ and does not introduce a growing discrete mode when $U\ne c$.

For real $k$, suppose $c=c_r+ic_i$ with $c_i\ne0$, so division by $U-c$ is legitimate. Multiply the [ordinary differential equation](../../../../../ordinary-differential-equation.md) by $\phi^*/[r(U-c)]$, integrate, and apply [integration by parts](../../../../../integration-by-parts.md). The endpoint terms vanish by the preceding regularity and wall conditions, leaving

$$
\int_0^a\frac{|\phi'|^2+k^2|\phi|^2}{r}\,dr+
\int_0^a\frac{(U'/r)'|\phi|^2}{U-c}\,dr=0.
$$

Taking its imaginary part yields

$$
c_i\int_0^a\frac{(U'/r)'|\phi|^2}{|U-c|^2}\,dr=0.
$$

**A growing temporal mode therefore requires a sign change of $(U'/r)'$, rather than a sign change of $U''$ alone.** This is the cylindrical counterpart of [Rayleigh's inflection-point theorem](../../../../../rayleigh-s-inflection-point-theorem.md). If this derivative vanishes identically, the positive first integral rules out a nontrivial growing real-wavenumber mode as well. Isolated zeros without a sign change do not make the second integral vanish for a nonzero regular mode.

For the parabolic [Poiseuille flow](../../../../../hagen-poiseuille-equation.md), $U'/r=-2U_0/a^2$ is constant. Under the specified exclusion of critical levels, division gives

$$
\phi''-\frac{\phi'}r-k^2\phi=0.
$$

Setting $\phi=rf$, or equivalently choosing $n=1$ in $r^{-n}\phi$, turns this into

$$
r^2f''+rf'-(k^2r^2+1)f=0.
$$

It is the [Modified Bessel differential equation](../../../../../modified-bessel-differential-equation.md) of order one. Hence $\phi=r[A I_1(kr)+B K_1(kr)]$. Since $rK_1(kr)$ tends to a nonzero constant at the axis, it gives a singular radial [velocity](../../../../../velocity.md) and must be excluded. The admissible [mode shape](../../../../../mode-shape.md) is therefore

$$
\boxed{\phi=A rI_1(kr),\qquad I_1(ka)=0}.
$$

For $k=0$, direct solution gives $\phi=C r^2$ after axis regularity, and the wall condition again forces the trivial solution. For nonzero $k$, the nonzero roots of $I_1$ are imaginary. Writing $j_{1,l}>0$ for the zeros of the ordinary [Bessel function](../../../../../bessel-function.md) $J_1$, the [evanescent potential modes of inviscid Poiseuille flow](../../../../../evanescent-potential-modes-of-inviscid-poiseuille-flow.md) are

$$
\boxed{k=\pm i j_{1,l}/a,\qquad \phi\propto rJ_1(j_{1,l}r/a)}.
$$

Their perturbation [vorticity](../../../../../vorticity.md) vanishes: $\partial_z u-\partial_r w=k^2\phi/r-(\phi'/r)'=0$. These modes grow exponentially in one axial direction and decay in the other. They can describe end-forced or spatially localized potential fields, but neither sign gives a bounded [normal mode](../../../../../normal-mode.md) on a whole infinite pipe. Moreover, the reduced radial equation contains no $c$: it supplies no temporal [eigenvalue](../../../../../eigenvalue.md) condition. An arbitrary imaginary part assigned to $\omega=kc$ here is consequently not evidence for a physical temporal instability.

The real-wavenumber calculation does exclude growing discrete axisymmetric modes of this inviscid profile. It does not establish every form of stability: singular neutral disturbances with $c$ in the range of $U$, transient dynamics, non-axisymmetric disturbances, and finite-amplitude transition require separate treatment. The exclusion $U\ne c$ specifically removes the inviscid continuous spectrum.

With [viscosity](../../../../../dynamic-viscosity.md), linearize the [Navier-Stokes equations](../../../../../navier-stokes-equation.md) instead and eliminate [pressure](../../../../../pressure.md) to obtain a fourth-order cylindrical counterpart of the [Orr-Sommerfeld equation](../../../../../orr-sommerfeld-equation.md). Impose both $\phi(a)=0$ and $\phi'(a)=0$, with appropriate regularity at the axis. The resulting [eigenvalue problem](../../../../../eigenvalue-problem.md) involves the [Reynolds number](../../../../../reynolds-number.md) and determines complex [frequencies](../../../../../frequency.md), rather than leaving $c$ arbitrary. Viscosity supplies diffusion, no-slip boundary layers and critical-layer regularization, so the inviscid sign argument alone no longer decides its spectrum. That observation does not imply that viscous pipe flow must have a growing linear eigenmode; finite-amplitude pipe transition is a different question.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 74](../../paper-74-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

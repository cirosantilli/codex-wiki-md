<h1 id="38b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Linearized mass conservation, momentum balance and the isentropic pressure-density relation are $\rho'_t+\rho_0\nabla\cdot\mathbf u=0$, $\rho_0\mathbf u_t=-\nabla\widetilde p$, and $\widetilde p=c_0^2\rho'$. Differentiate mass conservation in time and take the divergence of momentum balance to eliminate velocity. This gives the [acoustic pressure wave equation](../../../../../../acoustic-pressure-wave-equation.md)

$$
\boxed{\widetilde p_{tt}=c_0^2\nabla^2\widetilde p}.
$$

For the convention $\widetilde p=\operatorname{Re}e^{i(\mathbf k\cdot\mathbf r-\omega t)}$, momentum balance gives the complex velocity amplitude $\mathbf k/(\rho_0\omega)$, with $\omega=c_0|\mathbf k|$. Thus the incident [velocity field](../../../../../../velocity-field.md) is $\operatorname{Re}[\mathbf k_Ie^{i(\mathbf k_I\cdot\mathbf r-\omega t)}/(\rho_1\omega)]$ in the lower gas.

Let $a=k_I\sin\theta$, $l_1=k_I\cos\theta>0$, $\omega=c_1k_I$, and $l_2=\sqrt{(\omega/c_2)^2-a^2}$ with nonnegative real or imaginary part. This chooses an outgoing propagating wave or an evanescent wave decaying as $y\to+\infty$. Conservation of tangential [wavevector](../../../../../../wavevector.md) is the acoustic [Snell law for elastic and acoustic waves](../../../../../../snell-law-for-elastic-and-acoustic-waves.md). Write the complex pressures as

$$
p_1=e^{i(ax-\omega t)}(e^{il_1y}+R e^{-il_1y}),\qquad
p_2=T e^{i(ax+l_2y-\omega t)}.
$$

Inviscid kinematic matching requires equal normal velocities at the plate, not equal tangential velocities:

$$
\frac{l_1}{\rho_1\omega}(1-R)=\frac{l_2}{\rho_2\omega}T=-i\omega\eta_0.
$$

Define the [normal acoustic impedance](../../../../../../normal-acoustic-impedance.md) ratio $\delta=\rho_2l_1/(\rho_1l_2)$, so $T=\delta(1-R)$. For a propagating transmitted wave this is $\rho_2c_2\cos\theta/(\rho_1c_1\cos\theta_2)$. The dynamic condition gives

$$
T-1-R=(m\omega^2-Ba^4)\eta_0=i\beta(1-R),
\quad \beta=\frac{(m\omega^2-Ba^4)l_1}{\rho_1\omega^2},
$$

which is exactly the printed dimensionless parameter. Solving yields the pressure [reflection coefficient](../../../../../../reflection-coefficient.md) and [transmission coefficient](../../../../../../transmission-coefficient.md)

$$
\boxed{R=\frac{\delta-1-i\beta}{\delta+1-i\beta},\qquad
T=\frac{2\delta}{\delta+1-i\beta}}.
$$

At $l_2=0$ use the preceding velocity equations, or take their limit, rather than substituting an infinite $\delta$. For real $l_2>0$, the reflected [energy](../../../../../../energy.md) fraction is $|R|^2$, the transmitted fraction is $|T|^2/\delta$, and these sum to one. An evanescent transmitted wave carries no mean normal [energy](../../../../../../energy.md) flux.

When the gases match, $\delta=1$, so $R=-i\beta/(2-i\beta)$ and $T=2/(2-i\beta)$. For a nongrazing incident wave of nonzero frequency, perfect transmission means $R=0$, equivalent to

$$
\boxed{\beta=0\quad\Longleftrightarrow\quad m\omega^2=Bk_I^4\sin^4\theta
\quad\Longleftrightarrow\quad mc_0^2=Bk_I^2\sin^4\theta}.
$$

The plate's inertial and bending terms cancel: the incident frequency and tangential [wavevector](../../../../../../wavevector.md) coincide with its free [flexural wave](../../../../../../flexural-wave.md) [dispersion relation](../../../../../../dispersion-relation.md). Then $T=1$, including its phase. With positive $m,B$, this condition is possible only at angles and frequencies satisfying that relation; for normal incidence at nonzero frequency it cannot occur unless the mass is zero.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [38B](../../38b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

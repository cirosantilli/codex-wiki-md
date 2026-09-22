<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

**Potential-vorticity dynamics.** The [quasi-geostrophic potential-vorticity equation](../../../quasi-geostrophic-potential-vorticity-equation.md) expresses material conservation of a balanced [potential vorticity](../../../potential-vorticity.md) by a horizontally nondivergent [geostrophic flow](../../../geostrophic-flow.md). Its terms represent relative vorticity, planetary vorticity and the layer-thickness/free-surface contribution. The [Rossby deformation radius](../../../rossby-deformation-radius.md) $L_d$ measures the scale at which that thickness contribution competes with the horizontal-vorticity term. The [quasi-geostrophic approximation](../../../quasi-geostrophic-approximation.md) filters fast [acoustic waves](../../../acoustic-wave.md) and [gravity waves](../../../gravity-wave-split.md), making the slower balanced evolution accessible to early digital forecasts. The 1950 barotropic-vorticity forecasting study demonstrated practical twenty-four-hour forecasts from observed mid-tropospheric fields, while identifying [discretization](../../../discretization.md) and omitted [baroclinicity](../../../baroclinity.md) as error sources.[Abstract and introductory development: filtered geostrophic description; four 24-hour forecasts at 500 mb; forecast-error discussion](https://maths.ucd.ie/~plynch/eniac/CFvN-1950.pdf)

Near the north pole put $\delta=\pi/2-\theta$ and $r\simeq a\delta$. Then

$$
f=2\Omega\sin\theta=2\Omega\cos\delta\simeq2\Omega-\Omega\delta^2
=\boxed{2\Omega-\frac{\gamma r^2}2},\qquad \gamma=2\Omega/a^2.
$$

Using projected rather than arc distance gives the same leading polar expansion. It is a north-polar expression; the sign structure is changed consistently at the opposite pole.

In cylindrical coordinates, horizontal advection is $u_r\partial_rQ+(u_\phi/r)\partial_\phi Q$. Substituting the specified [streamfunction](../../../stream-function.md) gives

$$
\boxed{\partial_tQ+J(\psi,Q)=0,\qquad
J(\psi,Q)=\frac1r(\psi_rQ_\phi-\psi_\phi Q_r)}.
$$

The factors of $1/r$ are required by cylindrical geometry.

**An exact traveling eigenfunction.** This is a [polar gamma-plane Rossby wave](../../../polar-gamma-plane-rossby-wave.md). The radial equation implies $\nabla_h^2\psi-\psi/L_d^2=-\alpha^2\psi$, so $Q=f-\alpha^2\psi$. Since $J(\psi,\psi)=0$, its nonlinear self-advection vanishes exactly, regardless of amplitude. Also $f_r=-\gamma r$, giving $J(\psi,f)=\gamma\psi_\phi$. Hence

$$
-\alpha^2\psi_t+\gamma\psi_\phi=0.
$$

For $\psi=F(r)\cos(\omega t-n\phi)$, this yields

$$
\boxed{\omega=-\frac{n\gamma}{\alpha^2}}.
$$

The wave is retrograde relative to the balanced mean flow, since $\omega/n<0$ in this convention.

Multiplying the radial equation by $r^2$ gives

$$
r^2F''+rF'+[(\alpha^2-L_d^{-2})r^2-n^2]F=0.
$$

For $K^2=\alpha^2-L_d^{-2}>0$, setting $y=Kr$ gives the standard [Bessel equation](../../../bessel-differential-equation.md) with derivatives with respect to $y$. Thus

$$
\boxed{F(r)=C_1J_n(Kr)+C_2Y_n(Kr),\qquad K=\sqrt{\alpha^2-L_d^{-2}}}.
$$

Regularity at the pole excludes $Y_n$ for the usual nonnegative integers. If $K^2<0$, the corresponding general solutions are [modified Bessel functions](../../../modified-bessel-function.md); at $K=0$ they are $r^{\pm n}$, with a constant and $\ln r$ for $n=0$. The printed Bessel hint mixes its independent-variable labels; using $y=Kr$ and derivatives in $y$ resolves that notation.

**What the hexagon fixes.** With the north-polar approximation and the supplied rotation period,

$$
\Omega=\frac{2\pi}{37980\ \mathrm s}=1.654\times10^{-4}\ \mathrm{s^{-1}},\quad
r_0\simeq a\frac{14\pi}{180}=1.417\times10^7\ \mathrm m,\quad
\gamma=9.84\times10^{-20}\ \mathrm{m^{-2}\,s^{-1}}.
$$

The intrinsic phase speed at that radius is $c_\phi=r_0\omega/n=-\gamma r_0/\alpha^2$. Therefore the measured $-4\ \mathrm{m\,s^{-1}}$ fixes

$$
\boxed{\alpha^2=\frac{\gamma r_0}{4}=3.48\times10^{-13}\ \mathrm{m^{-2}},\qquad
L_d=(\alpha^2-K^2)^{-1/2}}.
$$

The [polar-wave deformation-radius identifiability](../../../polar-wave-deformation-radius-identifiability.md) issue is that a unique $L_d$ additionally requires a radial [wavenumber](../../../wavenumber.md) or boundary condition. The quoted peak-to-peak meander is an amplitude, not a radial wavelength: multiplying the exact eigenfunction by a constant changes its amplitude without changing $K,\alpha$ or $\omega$. Thus it cannot be silently converted into $K=2\pi/\Delta r$.

A transparent order-of-magnitude closure is a slowly varying radial envelope near $r_0$, so $F''+F'/r$ is small relative to $n^2F/r_0^2$. Then $K^2\simeq n^2/r_0^2$ and

$$
\boxed{L_d\simeq\left(\alpha^2-\frac{36}{r_0^2}\right)^{-1/2}\simeq2.4\times10^6\ \mathrm m}.
$$

This is a conditional estimate, not a uniquely determined observation. The general real-$K$ bound is $L_d\ge\alpha^{-1}\simeq1.7\times10^6$ m. Different radial structures give different values: for example $K=3.0\times10^{-7}$ and $5.0\times10^{-7}\ \mathrm{m^{-1}}$ yield about $2.0\times10^6$ and $3.2\times10^6$ m, respectively, at the same measured phase speed. Their amplitudes remain free. The given $5^\circ$ meander corresponds to a radial half-amplitude about $2.5\times10^6$ m and helps characterize the pattern's size, but alone removes none of this eigenvalue ambiguity.

## ↑ Ancestors (11)

1. [6](../6.md)
2. [2016](../../2016-split.md)
3. [Past exam of the physics of atmospheres and oceans course of the University of Oxford](../../split.md)
4. [Physics of atmospheres and oceans course of the University of Oxford](../../../physics-of-atmospheres-and-oceans-course-of-the-university-of-oxford.md)
5. [Year 4 of the physics course of the University of Oxford](../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)

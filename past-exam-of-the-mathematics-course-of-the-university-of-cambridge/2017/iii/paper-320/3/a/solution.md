<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

On a length scale $\ell$, [pressure](../../../../../../pressure.md) communicates support over a sound-crossing [time](../../../../../../time-in-physics.md) $\ell/v_s$, whereas self-gravity acts over a [time](../../../../../../time-in-physics.md) of order $(G\rho_0)^{-1/2}$. When the former is longer, gravity can amplify an overdensity before [pressure](../../../../../../pressure.md) smooths it. Thus [Jeans instability](../../../../../../jeans-instability.md) occurs at scales of order $\ell\gtrsim v_s/\sqrt{G\rho_0}$; the precise numerical factor depends on whether scale means [wavelength](../../../../../../wavelength.md) or inverse [wavenumber](../../../../../../wavenumber.md).

Take a uniform static background, small perturbations, an inviscid [barotropic fluid](../../../../../../barotropic-fluid.md), and $\delta p=v_s^2\delta\rho$ with $v_s^2=(dp/d\rho)_0>0$. An infinite Newtonian homogeneous density cannot itself have zero background gravitational [acceleration](../../../../../../acceleration.md) while satisfying the unmodified [Poisson equation for Newtonian gravity](../../../../../../poisson-equation-for-newtonian-gravity.md). Specify the [Jeans swindle](../../../../../../jeans-swindle.md): subtract the homogeneous field, or regard an external prescription as balancing it, and apply Poisson's equation only to perturbations. The linearized [continuity equation](../../../../../../continuity-equation.md) and [Euler equations for an inviscid fluid](../../../../../../euler-equations-for-an-inviscid-fluid.md) are

$$
\partial_t\delta\rho+\rho_0\nabla\cdot\delta\mathbf v=0,\qquad\partial_t\delta\mathbf v=-\frac{v_s^2}{\rho_0}\nabla\delta\rho-\nabla\delta\phi,\qquad\nabla^2\delta\phi=4\pi G\delta\rho.
$$

Taking a [time](../../../../../../time-in-physics.md) [derivative](../../../../../../derivative.md) of the first equation and substituting the second yields $\partial_t^2\delta\rho=v_s^2\nabla^2\delta\rho+4\pi G\rho_0\delta\rho$. A [plane wave](../../../../../../plane-wave.md) $e^{i(\mathbf k\cdot\mathbf x-\omega t)}$ therefore gives

$$
\boxed{\omega^2=v_s^2k^2-4\pi G\rho_0,\qquad k_J=\frac{\sqrt{4\pi G\rho_0}}{v_s}.}
$$

For $0<k<k_J$ there is exponential growth at rate $\sqrt{4\pi G\rho_0-v_s^2k^2}$. At $k_J$ the density mode is neutral to this linear order, and above it there are acoustic oscillations. The critical [wavelength](../../../../../../wavelength.md) is $2\pi/k_J=\sqrt\pi\,v_s/\sqrt{G\rho_0}$. Transverse [velocity](../../../../../../velocity.md) perturbations decouple as zero-frequency vortical modes in this idealization.

For the attractive [Yukawa potential](../../../../../../yukawa-potential.md), assume a real screening parameter $\alpha\geq0$. Its Green function obeys $(\nabla^2-\alpha^2)(-Gm e^{-\alpha r}/r)=4\pi Gm\delta^{(3)}(\mathbf r)$, including the delta source. Thus $\delta\phi_{\mathbf k}=-4\pi G\delta\rho_{\mathbf k}/(k^2+\alpha^2)$. The same fluid elimination gives [Jeans instability with Yukawa gravity](../../../../../../jeans-instability-with-yukawa-gravity.md):

$$
\boxed{\omega^2=k^2\left[v_s^2-\frac{4\pi G\rho_0}{k^2+\alpha^2}\right].}
$$

There exists a growing nonzero-wavenumber mode precisely when

$$
\boxed{4\pi G\rho_0>v_s^2\alpha^2,\qquad0<k<\sqrt{k_J^2-\alpha^2}.}
$$

Equality gives no exponentially growing nonzero mode. If screening exceeds this threshold, the finite-range gravitational response is too weak to overcome [pressure](../../../../../../pressure.md) at any [wavelength](../../../../../../wavelength.md). Otherwise all sufficiently long but nonconstant waves remain unstable, with a longer minimum unstable [wavelength](../../../../../../wavelength.md) than in Newtonian gravity. For $\alpha>0$ the long-wave gravitational contribution also scales as $k^2$, so the growth rate tends to zero as $k\to0$; screening does not produce a second positive lower cutoff in [wavenumber](../../../../../../wavenumber.md). A homogeneous screened background can have the constant [gravitational potential](../../../../../../newtonian-potential-of-a-point-mass.md) $-4\pi G\rho_0/\alpha^2$, with zero [force](../../../../../../force.md), so no Newtonian background subtraction is needed for nonzero screening. The limits $k\to0$ and $\alpha\to0$ are nonuniform. An exact $k=0$ density change is not one of the growing finite-wavelength modes. In the pressureless edge case $v_s=0$, every finite $k>0$ is unstable for positive density and finite screening.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 320](../../../paper-320-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A periodic pattern breaks continuous [translation symmetry](../../../../../translational-symmetry.md): translating it changes its [phase](../../../../../phase-waves.md) without changing its shape or its energy. Consequently a uniform [phase](../../../../../phase-waves.md) change is neutral. A slowly varying [phase](../../../../../phase-waves.md) change alters the local spacing or orientation and can grow even while ordinary uniform [amplitude](../../../../../wave-amplitude.md) perturbations decay. These are long-wavelength [sideband instabilities](../../../../../sideband-instability.md). The relevant wavelengths are long compared with the carrier pattern, so their leading dynamics is often a [phase modulation](../../../../../phase-modulation.md) equation. Positive [phase](../../../../../phase-waves.md) diffusion smooths spacing errors; negative [phase](../../../../../phase-waves.md) diffusion amplifies them. Near onset, an [amplitude equation](../../../../../amplitude-equation.md) computes this diffusion explicitly. Away from onset, one must calculate it from the full nonlinear periodic pattern.

For a supercritical stationary pattern in one dimension, rescale the [real Ginzburg–Landau equation](../../../../../real-ginzburg-landau-equation.md) to

$$
A_t=\mu A+A_{xx}-|A|^2A.
$$

A detuned periodic pattern is represented by $A=R e^{iqx}$, with $R^2=\mu-q^2>0$. Perturb its magnitude and [phase](../../../../../phase-waves.md) by $A=(R+u)e^{i(qx+\phi)}$. [Linearization](../../../../../linearization.md) gives

$$
u_t=-2R^2u+u_{xx}-2qR\phi_x,\qquad
\phi_t=\phi_{xx}+\frac{2q}{R}u_x.
$$

For a [Fourier mode](../../../../../fourier-mode.md) proportional to $e^{\lambda t+ikx}$, the two [eigenvalues](../../../../../eigenvalue.md) are the [sideband spectrum of a real Ginzburg-Landau plane wave](../../../../../sideband-spectrum-of-a-real-ginzburg-landau-plane-wave.md):

$$
\lambda_\pm=-R^2-k^2\pm\sqrt{R^4+4q^2k^2}.
$$

The magnitude branch remains damped at small $k$. The [phase](../../../../../phase-waves.md) branch expands as

$$
\lambda_+=-D_\parallel k^2+O(k^4),\qquad
D_\parallel=\frac{\mu-3q^2}{\mu-q^2}.
$$

Hence the **Eckhaus-stable band is $\boxed{q^2<\mu/3}$**, narrower than the existence band $q^2<\mu$. This [Eckhaus instability](../../../../../eckhaus-instability.md) is longitudinal: it compresses and dilates the pattern along its [wavevector](../../../../../wavevector.md). The coupling to the relaxing magnitude is crucial; examining [phase](../../../../../phase-waves.md) diffusion while holding the magnitude fixed would miss the destabilizing $2q^2/R^2$ correction. At the stability boundary the $k^2$ [coefficient](../../../../../coefficient.md) vanishes, and the next term is negative, $-2q^4k^4/R^6$. Beyond the boundary, a [phase](../../../../../phase-waves.md) distortion can create [amplitude](../../../../../wave-amplitude.md) zeros and [phase slips](../../../../../phase-slip.md), changing the number of periods. These nonlinear events are possible outcomes, not conclusions of the linear calculation.

A fixed periodic domain allows only discrete sideband [wavenumbers](../../../../../wavenumber.md). Indeed, the displayed spectrum is unstable only if $0<k^2<6q^2-2\mu$. A domain too short to support such a [Fourier mode](../../../../../fourier-mode.md) can suppress the nominal long-wave instability. Thus an infinite-domain stability band and a finite-domain threshold must be distinguished.

The [zigzag instability](../../../../../zigzag-instability.md) concerns transverse bending of rolls in an isotropic two-dimensional system. Let $k_c$ be the preferred carrier [wavenumber](../../../../../wavenumber.md), use an $x$-directed carrier, and denote its slow longitudinal detuning by $q$. Rotational covariance near onset leads to the anisotropic envelope equation

$$
A_t=\mu A+\xi\left(\partial_X-\frac{i}{2k_c}\partial_Y^2\right)^2A-g|A|^2A,\qquad\xi,g>0.
$$

The derivative combination comes from expanding $|\boldsymbol k|-k_c$: a small transverse carrier component changes the length of the [wavevector](../../../../../wavevector.md) only at second order. A straight-roll envelope $A=R e^{iqX}$ has $gR^2=\mu-\xi q^2$. For a purely transverse [phase](../../../../../phase-waves.md) perturbation $A\simeq R e^{iqX}(1+i\phi(Y,t))$, magnitude and [phase](../../../../../phase-waves.md) decouple at linear order, and

$$
\phi_t=\frac{\xi q}{k_c}\phi_{YY}-\frac{\xi}{4k_c^2}\phi_{YYYY}.
$$

The transverse [growth rate](../../../../../growth-rate.md) is therefore

$$
\boxed{\lambda_\perp=-\frac{\xi q}{k_c}k_Y^2-\frac{\xi}{4k_c^2}k_Y^4.}
$$

Rolls with $q<0$, whose total [wavenumber](../../../../../wavenumber.md) is below the preferred value, are zigzag-unstable to sufficiently long transverse modulations. Bending increases their local [wavevector](../../../../../wavevector.md) length and can relieve this mismatch. Rolls with $q>0$ are transversely stable in this near-onset model; at $q=0$ the restoring force first appears at fourth spatial order. Combining this with the longitudinal [Eckhaus instability](../../../../../eckhaus-instability.md) gives the robust interior stable band $0<q<\sqrt{\mu/(3\xi)}$ for this simplest isotropic roll model. Anisotropy, a pinned orientation, additional mean fields, or other pattern [symmetries](../../../../../symmetry-physics.md) can modify this conclusion.

For oscillatory patterns the [coefficients](../../../../../coefficient.md) of the [amplitude equation](../../../../../amplitude-equation.md) are generally complex. Consider the scaled [complex Ginzburg–Landau equation](../../../../../complex-ginzburg-landau-equation.md)

$$
A_t=A+(1+ic_1)A_{xx}-(1+ic_3)|A|^2A,
$$

where $c_1$ measures linear dispersion and $c_3$ the amplitude-dependent frequency shift. The uniform oscillation is $A=e^{-ic_3t}$. Put $A=e^{-ic_3t}(1+u+iv)$, with real infinitesimal $u,v$. The linearized magnitude and [phase](../../../../../phase-waves.md) equations are

$$
u_t=-2u+u_{xx}-c_1v_{xx},\qquad
v_t=-2c_3u+c_1u_{xx}+v_{xx}.
$$

Their [characteristic polynomial](../../../../../characteristic-polynomial.md) for a sideband of [wavenumber](../../../../../wavenumber.md) $k$ is

$$
\lambda^2+(2+2k^2)\lambda+2(1+c_1c_3)k^2+(1+c_1^2)k^4=0.
$$

The magnitude mode has leading [eigenvalue](../../../../../eigenvalue.md) $-2$, while the neutral [phase](../../../../../phase-waves.md) mode has

$$
\lambda=-(1+c_1c_3)k^2+O(k^4).
$$

Thus **the Benjamin-Feir instability occurs for $\boxed{1+c_1c_3<0}$**; the complementary [Benjamin-Feir stability condition](../../../../../benjamin-feir-stability-condition.md) is $1+c_1c_3>0$. Both dispersive couplings matter: the [phase](../../../../../phase-waves.md) perturbs the magnitude through $c_1$, and the magnitude feeds back into [phase](../../../../../phase-waves.md) through $c_3$. In the unstable regime, higher spatial derivatives regularize sufficiently short disturbances. On a finite domain, an unstable mode must satisfy $0<k^2<-2(1+c_1c_3)/(1+c_1^2)$. At equality of the phase-diffusion [coefficient](../../../../../coefficient.md) to zero, the leading [phase](../../../../../phase-waves.md) damping is fourth order, not exponential growth at order $k^2$.

Oscillatory plane waves with a nonzero carrier detuning also have a generalized Eckhaus boundary. For the [Ginzburg-Landau plane wave](../../../../../ginzburg-landau-plane-wave.md) $A=R e^{i(qx-\omega t)}$, one has $R^2=1-q^2$ and $\omega=c_1q^2+c_3R^2$. Eliminating the damped magnitude mode to second order in a sideband [wavenumber](../../../../../wavenumber.md) gives

$$
\lambda=-2i(c_1-c_3)qk-D(q)k^2+O(k^3),\qquad
D(q)=1+c_1c_3-\frac{2(1+c_3^2)q^2}{1-q^2}.
$$

The imaginary linear term transports the modulation; the sign of $D(q)$ determines its leading growth. If $1+c_1c_3>0$, the long-wave stable carrier band is

$$
q^2<\frac{1+c_1c_3}{3+c_1c_3+2c_3^2}.
$$

For $c_1=c_3=0$ this reduces to the real-equation Eckhaus band. If $1+c_1c_3<0$, even the zero-detuning oscillation has the [Benjamin-Feir instability](../../../../../benjamin-feir-instability.md). Nonlinear outcomes can include smooth [phase modulation](../../../../../phase-modulation.md), defect production or [phase](../../../../../phase-waves.md) turbulence, depending on the equation and parameters.

The general nonlinear-pattern problem starts from a periodic solution $u_0(x)$ of the full field equations, not from a small-amplitude envelope. Linearize about it to obtain an operator $L$ with periodic [coefficients](../../../../../coefficient.md). Write a disturbance as $e^{\lambda t+iq\cdot x}v(x)$ with $v$ periodic on the pattern cell. The [Bloch stability operator](../../../../../bloch-stability-operator.md)

$$
L(q)=e^{-iq\cdot x}Le^{iq\cdot x}
$$

acts on this fixed cell and determines the entire sideband spectrum. Translation covariance gives $L(0)\partial_xu_0=0$ in one dimension, and corresponding neutral directions for each independent broken translation in several dimensions. Oscillatory base patterns require the analogous [Floquet theory](../../../../../floquet-theory.md) calculation over their temporal period, or a rotating frame where applicable.

For a simple translational zero [eigenvalue](../../../../../eigenvalue.md), the phase-diffusion calculation can be made explicit. Expand

$$
L(q)=L_0+iqL_1-q^2L_2+\cdots,\quad
v(q)=v_0+iqv_1+O(q^2),\quad
\lambda(q)=icq-Dq^2+O(q^3),
$$

where $v_0=u_0'$ and $L_0v_0=0$. Choose an adjoint neutral function $w$ with $L_0^*w=0$, $\langle w,v_0\rangle=1$, and impose $\langle w,v_1\rangle=0$. First-order solvability, using the [Fredholm alternative](../../../../../fredholm-alternative.md), gives

$$
c=\langle w,L_1v_0\rangle,\qquad L_0v_1=cv_0-L_1v_0.
$$

At second order, applying the same adjoint solvability condition gives the [phase-diffusion coefficient from a Bloch cell problem](../../../../../phase-diffusion-coefficient-from-a-bloch-cell-problem.md):

$$
\boxed{D=\langle w,L_2v_0+L_1v_1\rangle.}
$$

This calculation exhibits why the nonlinear pattern profile matters: both $v_0$ and the cell correction $v_1$ depend on it. A negative $D$ signals a long-wave instability provided the rest of the spectrum is stable. With several [phase](../../../../../phase-waves.md) directions, or an extra neutral conserved mean, one obtains a coupled modulation system and diffusion matrices rather than this scalar formula. A two-dimensional [phase](../../../../../phase-waves.md) equation can schematically have $\phi_t=D_\parallel\phi_{xx}+D_\perp\phi_{yy}+\cdots$. Changing the sign of $D_\parallel$ gives the longitudinal [Eckhaus instability](../../../../../eckhaus-instability.md); changing the sign of $D_\perp$ gives the transverse [zigzag instability](../../../../../zigzag-instability.md). For oscillatory waves, nonvariational magnitude-phase coupling gives the [Benjamin-Feir instability](../../../../../benjamin-feir-instability.md).

These mechanisms extend beyond onset, but the near-onset numerical boundaries do not: their [coefficients](../../../../../coefficient.md) must be replaced by those obtained from the actual nonlinear pattern and its cell problems. Long-wave [linear stability](../../../../../linear-stability.md) is also only one part of stability; finite-wavenumber [eigenvalues](../../../../../eigenvalue.md), additional modes, defects, and boundary constraints can intervene. The unifying calculation is the splitting of translation-induced neutral modes at small modulation [wavenumber](../../../../../wavenumber.md), together with the coupling to the relaxing magnitude and any other slow fields.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 54](../../paper-54-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

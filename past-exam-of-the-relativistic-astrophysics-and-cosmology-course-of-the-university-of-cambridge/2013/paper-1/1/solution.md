<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For a blob in a [relativistic jet](../../../../relativistic-jet.md), take two emission events separated by time $\Delta t_e$ in the galaxy frame. The blob moves transversely by $u\Delta t_e\sin\theta$, while its second [photon](../../../../photon.md) has $u\Delta t_e\cos\theta$ less distance to travel to the distant observer. Therefore the arrival interval is $\Delta t_{\rm obs}=\Delta t_e(1-\beta\cos\theta)$ and

$$
\boxed{\beta_{\rm app}\equiv\frac{u_t}{c}=\frac{\beta\sin\theta}{1-\beta\cos\theta}}.
$$

Differentiating with respect to viewing angle gives $d\beta_{\rm app}/d\theta=\beta(\cos\theta-\beta)/(1-\beta\cos\theta)^2$. The maximum occurs at $\cos\theta=\beta$ and equals $\beta\gamma$. Hence [apparent superluminal motion](../../../../apparent-superluminal-motion.md) is possible precisely when $\beta\gamma>1$, or **$\beta>1/\sqrt2$**. This is an arrival-time effect; the material and every local signal still travel slower than [light](../../../../light.md).

<a id="1/image-original-arrival-time-geometry-and-apparent-transverse-speeds-for-subluminal-jet-velocities"></a>
![](../../../../past-exam-of-the-relativistic-astrophysics-and-cosmology-course-of-the-university-of-cambridge/2013/paper-1-jet-arrival.png)

**[Figure 1](#1/image-original-arrival-time-geometry-and-apparent-transverse-speeds-for-subluminal-jet-velocities). Original arrival-time geometry and apparent transverse speeds for subluminal jet velocities**.

For $\gamma\gg1$, $1-\beta\simeq1/(2\gamma^2)$ and $1-\beta\cos\theta\simeq(\gamma^{-2}+\theta^2)/2$. Thus the [Doppler factor](../../../../doppler-factor.md) is

$$
D\simeq\frac{2\gamma}{1+\gamma^2\theta^2}\longrightarrow\boxed{2\gamma}\quad(\theta\ll\gamma^{-1}).
$$

The [Lorentz-invariant specific intensity](../../../../lorentz-invariant-specific-intensity.md) gives $I_\nu/\nu^3=I'_{\nu'}/\nu'^3$. Since $\nu=D\nu'$, a [power-law spectrum](../../../../power-law-spectrum.md) with $I'_{\nu'}\propto\nu'^{-\alpha}$ gives $I_\nu(\nu)=D^3I'_{\nu'}(\nu/D)\propto D^{3+\alpha}$. This is [Doppler boosting of a moving blob](../../../../doppler-boosting-of-a-moving-blob.md): the [spectral flux density](../../../../spectral-flux-density.md) of an unresolved, intrinsically isotropic blob has the same boost. Comparing identical approaching and receding blobs, with no differential absorption,

$$
\frac{S_1}{S_2}=\left(\frac{D_1}{D_2}\right)^{3+\alpha}
=\boxed{\left(\frac{1+\beta\cos\theta}{1-\beta\cos\theta}\right)^4}\quad(\alpha=1).
$$

A spatially steady continuous jet can have a different boost exponent because the emitting material contributing at one arrival time differs; it must not silently replace the specified blob model.

Using the stipulated peak of the [photon-photon pair production](../../../../photon-photon-pair-production.md) [cross section](../../../../cross-section-physics.md), not the exact head-on threshold, gives

$$
\epsilon_{20}=\frac{2(m_ec^2)^2}{\epsilon_1}
=\frac{2(5.11\times10^5)^2}{5\times10^{11}}\,\mathrm{eV}
=\boxed{1.04\,\mathrm{eV}}.
$$

The relevant [photons](../../../../photon.md) are near [infrared](../../../../infrared.md). Interpret the quoted $F_2$ as target-band [energy](../../../../energy-split.md) flux, or [energy](../../../../energy-split.md) flux per logarithmic [frequency](../../../../frequency.md) interval, consistent with its units $\mathrm{W\,m^{-2}}$; it is not a [spectral flux density](../../../../spectral-flux-density.md) per hertz. For isotropic emission $L_2=4\pi d^2F_2$. In a stationary source of radius $R$, the order-of-magnitude [photon](../../../../photon.md) [energy density](../../../../energy-density.md) is $L_2/(4\pi R^2c)$, so

$$
n\sim\frac{F_2d^2}{R^2c\epsilon_{20}},\qquad
\tau\sim\frac{F_2d^2\sigma_T}{5Rc\epsilon_{20}}.
$$

The [luminosity variability size bound](../../../../luminosity-variability-size-bound.md) gives $R\lesssim c\Delta t$. Taking the largest allowed radius gives the smallest stationary-source [optical depth](../../../../optical-depth.md) in this estimate:

$$
\boxed{\tau_0\sim\frac{F_2d^2\sigma_T}{5\epsilon_{20}c^2\Delta t}}.
$$

This assumes the [gamma rays](../../../../gamma-ray.md) and target [photons](../../../../photon.md) occupy the same region, with an approximately isotropic target field and an order-unity geometric escape factor. A smaller region makes the [gamma-ray compactness problem](../../../../gamma-ray-compactness-problem.md) worse.

Here $d=3\times10^{25}\,\mathrm m$, $R\sim3\times10^{11}\,\mathrm m$, and $\epsilon_{20}=1.67\times10^{-19}\,\mathrm J$. Consequently

$$
\boxed{\tau_0\simeq3.2\times10^7\gg1}.
$$

Such a stationary co-spatial source would absorb almost all of its high-energy [photons](../../../../photon.md).

Let primes denote the blob [rest frame](../../../../rest-frame.md) and continue to ignore [cosmological redshift](../../../../cosmological-redshift.md). For fixed observed gamma-ray [energy](../../../../energy-split.md), $\epsilon'_1=\epsilon_1/D$. The co-moving target [energy](../../../../energy-split.md) at the assumed cross-section peak is therefore $\epsilon'_2=D\epsilon_{20}$. The [internal pair-production target energy in a relativistic blob](../../../../internal-pair-production-target-energy-in-a-relativistic-blob.md) acquires a second [Doppler shift](../../../../doppler-effect.md) when this same target population is observed along our [line of sight](../../../../line-of-sight.md):

$$
\boxed{\epsilon_{2,\rm obs}=D\epsilon'_2=D^2\epsilon_{20}}.
$$

It would be incorrect to transform only the [gamma ray](../../../../gamma-ray.md) while treating the internal target [radiation](../../../../radiation.md) as a stationary external field. The target [photons](../../../../photon.md) responsible for collisions span directions in the blob frame; the observed [energy](../../../../energy-split.md) here labels the corresponding part of the internally emitted [radiation spectrum](../../../../radiation-spectrum.md).

[relativistic beaming](../../../../relativistic-beaming.md) both increases the allowed rest-frame source radius, $R'\lesssim Dc\Delta t$, and lowers the inferred rest-frame [luminosity](../../../../luminosity.md), $L'_{\log}\sim L_{{\rm iso},\log}/D^4$. The [beamed gamma-ray optical depth](../../../../beamed-gamma-ray-optical-depth.md) then follows from $\epsilon'_2=D\epsilon_{20}$:

$$
\tau'(D)\sim\tau_0D^{-6}
\frac{F_{\log}(D^2\epsilon_{20})}{F_{\log}(\epsilon_{20})}.
$$

For an unbroken [power-law spectrum](../../../../power-law-spectrum.md) $F_\nu\propto\nu^{-\alpha}$, $F_{\log}=\nu F_\nu\propto\nu^{1-\alpha}$, so $\tau'\propto D^{-(4+2\alpha)}$. In particular, $\alpha=1$ gives the stated $D^{-6}$. Spectral breaks, an external target field or non-coincident emission regions change this inference. Under the requested scaling, transparency requires

$$
D\gtrsim\tau_0^{1/6}\simeq17.8,\qquad
\boxed{\gamma_{\min}\simeq8.9}.
$$

This minimum uses the most favourable nearly axial view, $D\simeq2\gamma$. The exact axial relation gives $\gamma_{\min}=(D_{\min}+D_{\min}^{-1})/2\simeq8.94$; a less favourable viewing angle requires a larger [Lorentz factor](../../../../lorentz-factor.md). The numerical bound is conditional on the stipulated opacity scaling and internal-source geometry.

## ↑ Ancestors (13)

1. [1](../1.md)
2. [Paper 1](../../paper-1-split.md)
3. [2013](../../split.md)
4. [Past exam of the relativistic Astrophysics and Cosmology course of the University of Cambridge](../../../split.md)
5. [Relativistic Astrophysics and Cosmology course of the University of Cambridge](../../../../relativistic-astrophysics-and-cosmology-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)

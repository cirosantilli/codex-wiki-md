# Ionospheric interference fringe spacing

↑ **Parent:** [Appleton-Barnett radio interference experiment](appleton-barnett-radio-interference-experiment.md)

Consider an original two-path model with a locally flat ground baseline $d$ and a symmetric equivalent return height $h$. Replace the [skywave](skywave.md) by two straight segments traveling at the [speed of light](speed-of-light.md) $c$, and replace the [ground wave](ground-wave.md) by a straight segment of length $d$. Their lengths and positive excess distance are

$$
L_s=2\sqrt{h^2+(d/2)^2},\qquad L_g=d,\qquad \Delta L=L_s-L_g>0.
$$

This is an equivalent geometric construction, not a metallic layer overhead. It neglects the curvature of [Earth](earth.md), [refraction](refraction.md) within the return region, ground-induced [wave phase](phase-waves.md) shifts and [optical dispersion](dispersion-optics.md).

For received [complex amplitudes](complex-amplitude.md) $A_g$ and $A_s$, absorb their constant relative [wave phase](phase-waves.md) into $\phi_0$ and choose their magnitudes nonnegative. An ideal detector reading proportional to squared received field has

$$
P(f)=K\left[A_g^2+A_s^2+2A_gA_s\cos\Phi(f)\right],\qquad
\Phi(f)=\frac{2\pi f\Delta L}{c}+\phi_0,\qquad K>0.
$$

Assume $\Delta L$ and $\phi_0$ are independent of [frequency](frequency.md) across the sweep, with slowly changing amplitudes. Consecutive maxima differ by $2\pi$ in [phase difference](phase-difference.md), so

$$
\Phi(f+\Delta f)-\Phi(f)=\frac{2\pi\Delta f\Delta L}{c}=2\pi,
\qquad \Delta f=\frac{c}{\Delta L}.
$$

The often-used approximation $\Delta f\simeq c/\Delta L$ therefore carries a frequency-independent-path assumption. Counting $N$ complete fringe periods between $f_1$ and $f_2$ gives $\Delta L\simeq Nc/|f_2-f_1|$; equivalently, $N=\Delta L|1/\lambda_2-1/\lambda_1|$ when the vacuum [wavelength](wavelength.md) is $\lambda=c/f$. Count whole periods, not maxima plus minima as though each were a whole period.

Choose $d=150\,\mathrm{km}$ and $h=100\,\mathrm{km}$, with $c\simeq3.00\times10^8\,\mathrm{m\,s^{-1}}$. Then $L_s=250\,\mathrm{km}$, $\Delta L=100\,\mathrm{km}$ and $\Delta f=3.00\,\mathrm{kHz}$. A $12.0\,\mathrm{kHz}$ sweep covers four full fringe periods. Conversely, the inferred equivalent height is

$$
h=\frac12\sqrt{(d+\Delta L)^2-d^2}=100\,\mathrm{km}.
$$

These chosen values illustrate the inversion; they are not a transcription of the 1924 measurements. With $A_g=1$ and $A_s=0.7$, the normalized reading ranges from $(1-0.7)^2=0.09$ to $(1+0.7)^2=2.89$: incomplete cancellation does not remove the distance information.

<a id="image-two-arrival-paths-and-the-interference-fringes-produced-by-a-controlled-frequency-sweep"></a>
![](ionosphere-ground-sky-interference.png)

**[Figure 5](#image-two-arrival-paths-and-the-interference-fringes-produced-by-a-controlled-frequency-sweep). Two arrival paths and the interference fringes produced by a controlled frequency sweep**. An original functional diagram distinguishes a curved skywave from a dashed equivalent straight-ray construction. The neighboring graph uses the stipulated nondispersive 150 km baseline and 100 km equivalent height, giving 3 kHz fringe spacing. The receiver detects the superposed arrivals.

For a sweep with linearly changing [frequency](frequency.md) $f(t)=f_0+\dot f t$ and two constant delays $\tau_s>\tau_g$, the received instantaneous [frequency](frequency.md) difference has magnitude $|\dot f|(\tau_s-\tau_g)$. In this model $\tau_s-\tau_g=\Delta L/c$, giving a [beat](beat.md) [frequency](frequency.md) $|\dot f|\Delta L/c$. Equivalently, traversing each $\Delta f$ of the sweep crosses one fringe. This calculation requires a sufficiently slow sweep that propagation, tuning and amplitude changes can be treated consistently; it is not a [beat](beat.md) between two independent transmitters.

More generally, measure the total [phase difference](phase-difference.md) $\Phi(f)$, including propagation and any reflection or apparatus contribution. Define the differential [group delay](group-delay.md)

$$
\Delta\tau_g=\frac{1}{2\pi}\frac{d\Phi}{df}.
$$

For a locally monotone [wave phase](phase-waves.md) with slowly varying [derivative](derivative.md), the local spacing is $\Delta f\simeq1/|\Delta\tau_g|$. If $\Phi=2\pi fD(f)/c+\phi_r(f)$, this becomes

$$
\Delta\tau_g=\frac{D+fD'}{c}+\frac{1}{2\pi}\phi_r'(f).
$$

Here $D(f)$ is a phase-equivalent [optical path difference](optical-path-difference.md), not necessarily the geometric excess distance $\Delta L$. A drifting [ionosphere](ionosphere.md), several simultaneous [skywaves](skywave.md), changing [wave polarization](polarization-waves.md), a frequency-dependent reflection [wave phase](phase-waves.md) or significant loss can invalidate the simple constant-spacing inversion.

## ↑ Ancestors (7)

1. [Appleton-Barnett radio interference experiment](appleton-barnett-radio-interference-experiment.md)
2. [Ionosphere](ionosphere.md)
3. [Upper atmosphere](upper-atmosphere.md)
4. [Geophysics](geophysics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Appleton-Barnett radio interference experiment](appleton-barnett-radio-interference-experiment.md)
